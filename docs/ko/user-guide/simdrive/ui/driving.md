# 차량 정보 UI
 차량의 주행 상태 및 제어 모드를 나타내는 **차량 정보 UI** 에 대해 설명합니다.
 
---

## 차량 정보 UI 접근하기
시뮬레이터 화면에서 Ego 차량을 마우스 클릭(🖱️)하면 화면 우측에 아래와 같은 차량 정보 패널이 나타납니다.

![uidefault](../../img/simdrive-ui-drivinginfo.png){:onclick="window.open(this.src)" width="500px" title="Click view screen" width="1000px"}
<figcaption><center><b> 그림 1. 차량 정보 UI</b></center></figcaption>

차량 정보 UI는 크게 **Graph** 와 **Driving Info** 탭으로 구성됩니다. 또한 시뮬레이터 상에 존재하는 Ego 차량 및 Sur 차량(주변 차량) 별로 각기 다른 **Graph** 와 **Driving Info** 를 확인할 수 있습니다.

???+ tip
    Ego 차량과 Sur 차량 간의 정보를 전환하려면 차량 정보 패널 상단 좌측의 아래와 같은 차량 아이콘을 클릭합니다. 

    ![uidefault](../../img/simdrive-ui-vehicleinfocon.png){:onclick="window.open(this.src)" title="Click view screen" width="500px"}
    <br>


<Br>
### Graph 탭
차량 정보 패널에서 좌측 **Graph** 탭을 클릭하면 주행 중인 차량의 제어 상태(가속, 브레이크, 조향 유무), 현재 속도, 가속도, 회전 각속도(Yaw Rate) 값을 아래와 같이 실시간 그래프로 확인할 수 있습니다.

![uidefault](../../img/simdrive-ui-vehicleinfogrh.png){:onclick="window.open(this.src)" width="500px" title="Click view screen" width="1000px"}
<figcaption><center><b> 그림 2. 주행 차량(Ego 및 Sur 차량)의 Graph UI 구성</b></center></figcaption>

<Br>
### Driving Info 탭
차량의 주행 옵션, 주행 상태 정보, 교통 정보를 Ego 및 Sur 차량 별로 표시한다.

#### Ego 차량의 Driving Info


#### Sur 차량의 Driving Info