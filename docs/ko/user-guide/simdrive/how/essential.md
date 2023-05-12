# 필수 정보
시뮬레이터를 사용하기에 앞서, 시뮬레이터 기준 좌표 및 모델 규격과 같이 반드시 숙지해야 할 필수 정보에 대해 설명합니다.

---

## 좌표계
시뮬레이터의 차량, 센서, 맵에서 사용하는 좌표계(Coordinate System)를 설명합니다. <br>
각 좌표계에 적용된 기준과 좌표값을 해석하는 방법을 설명합니다.

<br>

### 위치 좌표계
시뮬레이터에서 차량의 위치 및 차량에 장착하는 센서의 위치를 나타내는 좌표계에 대해 설명합니다. 아래 좌표계를 기준으로 나타냅니다.

<br>

#### 차량 위치 좌표계
시뮬레이터에서 차량 위치는 맵의 원점을 기준으로 ENU 좌표계로 나타냅니다. 또한 차량의 위치를 좌표깂으로 계산할 때는 멥의 원점에서부터 해당 차량의 후륜축 중심점까지의 거리를 계산합니다.

예를 들어, 시뮬레이터에서 Ego 차량을 최초 배치(단축키: `i`)했을 때 위치 좌표는 아래 그림과 같습니다. 

![uidefault](../../img/carcenter3.png)
<figcaption><center><b>그림 1. 시뮬레이터의 차량 스폰 위치 좌표</b></center></figcaption>

???+ tip
    차량의 최초 배치되는 위치 좌표는 차량 후륜축 중심에 GPS 센서를 장착 후, 아래와 같이 검출되는 GPS 데이터(위/경도 값)을 시뮬레이터 기준의 UTM 좌표계로 변환 후, 해당 UTM offset 값을 빼주어 계산합니다.

    ![uidefault](../../img/carcenter-gps.png)

<br>

???+ note
    ENU 좌표계를 기준으로, 시뮬레이터의 차량 방향은 아래와 같이 나타냅니다.

      - **21년 4월 9일 배포 버전** 부터는
        - 차량 헤딩 방향은 동쪽이다.
        - 차량 헤딩 각도는 동쪽을 0도로 두고, 반시계 방향(CCW)으로 증가(+)한다. 
        
      - **21년 3월 25일 배포 버전** 까지는:
        - 차량 헤딩 방향은 북쪽이다.
        - 차량 헤딩 각도는 북쪽을 0도로 두고, 반시계 방향(CCW)으로 증가(+)한다. 

<br>

#### 센서 위치 좌표계
차량에 장착하는 센서의 위치 좌표 (x, y, z)는  아래와 같은 시뮬레이터에서 바라보는 차량의 원점 및 각 방향 축을 기준으로 나타냅니다. 

  - 원점: 센서를 장착하는 Ego 차량의 뒷바퀴 후륜축 중심
  - x축: 지면과 평행한 축으로 y축과 수직임
  - y축: 뒷바퀴 축
  - z축: 지면에 수직인 축
  
![uidefault](../../img/sensorone.png)
<figcaption><center><b>그림 2. 시뮬레이터의 센서 위치 좌표계</b></center></figcaption>

<br>
### 센서 좌표계

시뮬레이터에서 제공하는 센서 모델의 특성에 맞추어, 각 센서를 차량에 장착할 때의 기준으로 하는 좌표계와 이에 따른 센서의 출력 데이터를 확인하는 방법을 설명합니다.


<br>

#### IMU 좌표계
IMU 센서를 차량에 장착할 시, 아래와 같은 6 자유도계의 값을 고려합니다.

  - x, y, z, roll, pitch, yaw

    <table>
      <tr>
        <td><img src="../../../img/imucoord1.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)" />
        </td>
        <td><img src="../../../img/imucoord2.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)" /></td>
      </tr>
    </table>  

IMU 좌표계를 기준으로 IMU 센서에서 검출하는 각 데이터의 좌표값은 아래와 같습니다.

  - **Linear_acceleration**
    - X: IMU 센서의 X 축에 대한 가속도 (전진 +, 후진 -)

    - Y: IMU 센서의 Y 축에 대한 가속도 (좌 +, 우 -)

    - Z: IMU 센서의 Z 축에 대한 가속도 (위 +, 아래 -)
<Br>

  - **Angular_velocity**

    - X: IMU 센서의 X 축에 대한 각속도 (Roll)

    - Y: IMU 센서의 Y 축에 대한 각속도 (Pitch)

    - Z: IMU 센서의 Z 축에 대한 각속도(Yaw)

    ???+tip
        회전축인 각 x, y, z 축을 기준으로 반 시계 방향이 `+`이고, 시계 방향은 `-`이다.
<br>

  - **Orientation**

    - X: Quaternion X 벡터

    - Y: Quaternion Y 벡터

    - Z: Quaternion Z 벡터

    - W: Quaternion w 벡터

<br>

#### GPS 좌표계
 GPS 센서에서 검출하는 좌표값은 아래와 같은 UTM 좌표계을 기준으로 계산합니다.

- **UTM52N** (WGS84)
  ```
    EPSG:32652
    +proj=utm +zone=52 +ellps=WGS84 +datum=WGS84 +units=m +no_defs
  ```

<br>

#### Velodyne LiDAR 좌표계
Velodyne LiDAR 센서에서 검출하는 좌표는 아래와 같이 축 방향을 가지는 값으로 구성됩니다.

- x: right
- y: forward
- z: up

각 좌표값은 아래의 Velodyne LiDAR의 채널 별 좌표 정보를 참고하여 계산합니다.

  <table>
    <tr>
      <td><img src="../../../img/essential-lidar1.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)" />
        <figcaption><center><b>16 Ch. LiDAR</b></center></figcaption>
      </td>
      <td><img src="../../../img/essential-lidar2.png"" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)"/>
        <figcaption><center><b>32 Ch. LiDAR</b></center></figcaption>
      </td>
    </tr>
    <tr>
      <td><img src="../../../img/essential-lidar3.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)" />
        <figcaption><center><b>64 Ch. LiDAR</b></center></figcaption>
      </td>
      <td><img src="../../../img/essential-lidar4.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)" />
      <br>
      <figcaption><center><b>128 Ch. LiDAR</b></center></figcaption>
      </td>
    </tr>
  </table>

시뮬레이터의 LiDAR 센서 좌표값을 ROS 통신으로 전송하는 경우 아래와 같은 ROS 특성 정보를 확인합니다.

- ROS Axis Orientation: [ROE 103 (ROS Enhancement Proposals)](https://www.ros.org/reps/rep-0103.html)의 ROS 표준 단위를 확인하면 아래와 같은 ROS의 기본 좌표계 정보를 확인할 수 있습니다.
    - x: forward
    - y: left
    - z: up

- ROS Velodyne Driver: 센서 데이터를 ROS 통신으로 전송하여 출력하려면 데이터를 수신하는 서버에 ROS Velodyne Driver를 설치해야 합니다. 이 때  센서 좌표값은   Velodyne LidDAR 좌표계(x: right y: forward  z: up)가 아닌 ROS 기본 좌표계(x: forward y: right z: up) 기준으로 출력됩니다.

시뮬레이터에서 Ego 차량의 LiDAR 센서가 인지하는 주변 환경에 대한 검출 데이터를 ROS 통신으로 수신했을 때 Velodyne의 Veloview와 ROS Rviz에서 시각화한 각 결과는 아래와 같습니다. 

![uidefault](../../img/essential-lidar-sim.png)
<figcaption><center><b>시뮬레이터의 센서 인지 환경</b></center></figcaption>
<br>
<table>
    <tr>
      <td><img src="../../../img/essential-lidar-vel.png" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)" />
        <figcaption><center><b>16 Ch. LiDAR</b></center></figcaption>
      </td>
      <td><img src="../../../img/essential-lidar-ros.png" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)"/>
        <figcaption><center><b>32 Ch. LiDAR</b></center></figcaption>
      </td>
    </tr>
    <tr>
      <td><img src="../../../img/essential-lidar-vel2.png" alt="sensor" style="width: 500px; height: auto;" title="Click to Enlage" onclick="window.open(this.src)" />
        <figcaption><center><b>64 Ch. LiDAR</b></center></figcaption>
      </td>
      <td><img src="../../../img/essential-lidar-ros2.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)" />
        <br><br>
        <figcaption><center><b>128 Ch. LiDAR</b></center></figcaption>
      </td>
    </tr>
  </table>

<br>
###  맵 좌표계
시뮬레이터의 맵에서 기준으로 하는 좌표계에 대해서 설명합니다.

시뮬레이터 내 존재하는 모든 객체의 위치는 [차량 위치 좌표](#_4)처럼, 아래와 같은 ENU 좌표계로 나타냅니다. 

![uidefault](../../img/mapenu.png)
<figcaption><b>그림 3. 시뮬레이터 맵 좌표계</b></figcaption>

???+ tip
    시뮬레이터 내 ENU 좌표 값을 확인하려면 원하는 화면 위치에 마우스 스크롤을 클릭합니다. 자세한 사용법은 [유용한 사용팁의 좌표 표시 기능](../useful/#_2)을 참고하십시오.


이러한 ENU 좌표값을 실제 지구 상에 위치하는 좌표값으로 변환하고자 할 때는 세계에서 통용되고 있는 투영좌표계인 [UTM 좌표계](https://ko.wikipedia.org/wiki/UTM_%EC%A2%8C%ED%91%9C%EA%B3%84)를 기준으로 계산합니다.

???+ tip
    시뮬레이터 맵에서 기준으로 하는 UTM 좌표 정보를 확인하려면 시뮬레이터 우측 하단의 맵 아이콘을 클릭합니다. 자세한 사용법은 [클러스터 및 맵 정보 UI 구성의 맵정보](../../ui/clustermap/#ui_2)를 확인하십시오.

시뮬레이터 맵에서 기준으로 하는 UTM 좌표 정보의 예시는 아래와 같습니다.
  
    {"isUtm":true,"utnNum":52,"utmOffset":{"x":302459.942,"y":4122635.537,"z":28.991},"projData":{"SPHEROID":"WGS84","LatitudeOfOrigin":0.0,"CentralMeridian":0.0,"ScaleFactor":1.0,"FalseEasting":0.0,"FalseNorthing":0.0}}


## 맵과 차량 모델 사양
시뮬레이터에서 제공하는 맵과 차량 모델의 사양 정보에 대해 설명합니다.
