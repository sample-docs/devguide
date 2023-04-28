# 클러스터 및 맵 정보 UI
주행 차량의 클러스터 및 맵 정보를 표시하는 UI에 대해 설명합니다.

---

## 클러스터 및 맵 정보 접근하기

시뮬레이터 기본 화면 UI 요소 중 상단 좌측 **톱니바퀴**(**⚙️**) > **Viewport Setting** 에서 **Show Vehicle Cluster and Map Info** 를 클릭합니다.

![uidefault](../../img/simdrive-ui-clumap.png){:onclick="window.open(this.src)" width="500px" title="Click view screen"}
<figcaption><b> 그림 1. 클러스터 및 맵 정보 메뉴</b></figcaption>

<br>
주행 차량의 클러스터 및 맵 정보가 아래와 같이 시뮬레이터 하단 상태바 위에 표시됩니다.

![uidefault](../../img/simdrive-ui-clumap2.png){:onclick="window.open(this.src)" title="Click view screen"}
<figcaption><center><b>그림 2. 클러스터 및 맵 정보 UI</b></center></figcaption>

<Br>
## 클러스터 정보

주행 차량의 클러스터 정보는 아래와 같이 **1] 차속 및 기어 상태**, **2] 조향 상태**, **3] 주행 차량 모델**, **4] 주행 요약 정보** 로 구성됩니다. 
<Br> 또한 하단 맨 좌측의 **5] △** 아이콘을 클릭하면 필요한 정보만 선택하여 표시할 수 있습니다.

![uidefault](../../img/simdrive-ui-clu.png){:onclick="window.open(this.src)" title="Click view screen"}
<figcaption><center><b>그림 2. 클러스터 및 맵 정보 UI</b></center></figcaption>


**1] 차속 및 기어 상태**: 차량의 현재 주행 속도(km/h)와 기어단(P/R/N/D) 정보 표시 <br>
**2] 조향 상태**: 차량 주행 방향을 휠 각도(deg, -36.3° ~ 36.3°)와 핸들 각도(deg, -450° ~ 450°)로 표시 <br>
 **3] 주행 차량 모델**:  Ego 차량의 모델 정보 표시 <br>
 **4] 주행 요약 정보**: 주행 정보를 가속 및 브레이크 유무, 휠 각도로 표시

???+ tip
    주행 요약 정보에서 가속 및 브레이크 유무는 1 또는 0으로만 표시합니다.
