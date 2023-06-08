# 기본 사용법

시뮬레이터의 **Sensor Edit Mode** 에서 센서를 장착(추가) 및 제거, 설정하는 방법을 설명합니다.

---

## Sensor Edit Mode 접근
Ego 차량에 센서를 장착 및 설정하려면 아래와 같이 상단 툴바에서 **Edit > Sensor > Sensor Edit Mode (단축키 F3)** 를 클릭합니다.
![uidefault](../../img/simdrive-how-sensoredit.png)
<figcaption><center><b>그림 1. Sensor Edit Mode 경로</b></center></figcaption>

아래와 같이 Ego 차량 좌측의 센서 설정창에서 원하는 센서를 장착 및 설정할 수 있습니다.
![uidefault](../../img/simdrive-how-sensoreditor.png)


## 센서 장착 및 추가
**1]** 센서 설정창에서 센서 종류를 선택 후 `Shift` 키를 누른 상태에서 장착하고자 하는 차량 위치에 마우스 클릭합니다.
![uidefault](../../img/simdrive-how-sensoradd.png)

**2]** 아래와 같이 장착 위치에 센서 좌표가 생기는 동시에, 하단에 해당 센서 설정을 위한 센서 속성창(**Sensor Properties**)이 나타납니다.
![uidefault](../../img/simdrive-how-sensorsetting.png)

장착한 센서의 종류는 **Sensor Properties** > **Active List** 탭에서 확인할 수 있습니다. 

다른 종류의 센서를 추가할 경우 위 **1], 2]** 과정을 반복합니다.

## 센서 제거
장착한 센서는 아래와 같은 방법 중 하나로 제거할 수 있습니다.

- **Sensor Properties > Sensor Settings** 에서 **Delete** 클릭 
  ![uidefault](../../img/simdrive-how-sensorsetting3.png){:onclick="window.open(this.src)" title="Click view screen" width="300px"}

-	**Sensor Properties > Active List** 에서 해당 센서에 대한 **휴지통 아이콘** 클릭
  ![uidefault](../../img/simdrive-how-sensorsetting4.png)


## 센서 설정
아래와 같이 **Sensor Properties > Sensor Settings** 탭에서 장착한 센서에 대한 입력 파라미터를 설정합니다. 
![uidefault](../../img/simdrive-how-sensorsetting1.png)

<Br>
아래의 방법 중 하나로 장착한 센서에 대한 **Sensor Settings** 으로 이동합니다.

- **Sensor Settings** 의 좌측 패널에서 장착한 센서와 매칭하는 아이콘 클릭
  ![uidefault](../../img/simdrive-how-sensorsetting2.png){:onclick="window.open(this.src)" title="Click view screen" width="300px"}

- **Sensor Properties > Active List** 에서 해당 센서에 대한 **설정 아이콘 (⚙️)** 클릭
  ![uidefault](../../img/simdrive-how-sensorsetting2-2.png){:onclick="window.open(this.src)" title="Click view screen" width="500px"}

각 센서 별 **Sensor Settings** 에서는 센서의 장착 위치 및 회전각, 센서 모델, 검출 데이터 형식(Groud Truth), 네트워크 등을 설정합니다. 

## 설정 정보 저장하기 및 불러오기 
 **Sensor Properties > Active List** 탭에서 하단의 **Load** 및 **Save** 버튼으로 센서의 설정 정보를 불러오거나 저장할 수 있습니다.

![uidefault](../../img/simdrive-sensorload.png)
<figcaption><center><b>그림 2. Sensor 설정 정보 저장하기 및 불러오기</b></center></figcaption>

센서 설정 정보를 불러오려면 **Load** 를 클릭하여 아래와 같이 **Sensor File Manager** 를 실행합니다.
![uidefault](../../img/simdrive-sensorload2.png)

**Sensor File Manager** 에서는 현재 실행 중인 시뮬레이터의 데이터 저장 경로에 존재하는 센서 설정 파일 리스트를 보여주며, 각 파일을 선택하여 시뮬레이터로 불러오거나 삭제할 수 있습니다. 

???+ tip
    시뮬레이터의 데이터 저장 경로는 
    `{시뮬레이터 설치 위치}\MoraiLauncher_Win\MoraiLauncher_Win_Data\SaveFile\Sensor\{실행 시뮬레이터 버전}`

<br>
센서 설정 정보를 저장하려면 **Save** 를 클릭하여 아래와 같이 **Save Sensor** 를 실행합니다.
![uidefault](../../img/simdrive-sensorload3.png)

센서 설정 정보는 `json` 파일 형태로 불어올 때와 동일한 경로에 저장됩니다.