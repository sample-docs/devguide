# 클러스터 및 맵 정보 UI
차량의 주행 정보 및 맵 정보를 계기 판넬로 보여주는 **클러스터 및 맵 정보 UI** 에 대해 설명합니다.

---

## Cluster and Map Info UI 접근
시뮬레이터 기본 화면 UI 요소 중 상단 좌측 **톱니바퀴**(**⚙️**) > **Viewport Setting** 에서 **Show Vehicle Cluster and Map Info** 를 클릭합니다.
![uidefault](../../img/simdrive-ui-clumap.png){:onclick="window.open(this.src)" width="500px" title="Click view screen"}
<br>


차량의 클러스터 및 맵 정보가 아래와 같이 시뮬레이터 하단 상태바 위에 표시됩니다.
![uidefault](../../img/simdrive-ui-clumap2.png){:onclick="window.open(this.src)" title="Click view screen"}
<figcaption><center><b>그림 1. Cluster and Map Info UI</b></center></figcaption>

## Cluster and Map Info UI  구성
차량의 클러스터 및 맵 정보는 아래와 같이 **1] 차속 및 기어 상태**, **2] 조향 상태**, **3] 주행 차량 모델**, **4] 주행 요약 정보**, **5] 맵 정보** 로 구성됩니다. 
<Br> 또한 하단 맨 좌측의 **6] △** 아이콘을 클릭하면 필요한 클러스터 및 맵 정보만 표시하도록 선택할 수 있습니다.
![uidefault](../../img/simdrive-ui-clumapinfo.png){:onclick="window.open(this.src)" title="Click view screen"}
<figcaption><center><b>그림 2. Cluster and Map Info UI 구성</b></center></figcaption>

**1] 차속 및 기어 상태**: 차량의 현재 주행 속도(km/h)와 기어단(P/R/N/D) 정보 표시 <br>
**2] 조향 상태**: 주행 방향을 휠 각도(deg, -36.3° ~ 36.3°)와 핸들 각도(deg, -450° ~ 450°)로 표시 <br>
**3] 주행 차량 모델**:  Ego 차량의 모델 정보 표시 <br>
**4] 주행 요약 정보**: 주행 정보를 가속 및 브레이크 유무, 휠 각도로 요약하여 표시 <br>

???+ tip
    주행 요약 정보에서 가속 및 브레이크 유무는 1 또는 0으로만 표시합니다.

 **5] 맵 정보**: 현재 맵 모델명 및 좌표 정보 

???+ tip
    **5] 맵 정보** 를 클릭하면 해당 맵에 대한 UTM offset 좌표 정보 (x, y, x)가 복사되어 아래와 같은 팝업 창이 나타납니다. 
    ![uidefault](../../img/simdrive-ui-mapinfo.png){:onclick="window.open(this.src)" title="Click view screen"}
    <br>

    맵 정보는 현재 시뮬레이터 상의 원점 정보로 매핑되며, 해당 offset 정보를 가지고 WGS84 좌표계(위도 및 경도)로 변환할 수 있습니다.

