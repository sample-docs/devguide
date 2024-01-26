# MORAI SIM 소개
**MORAI SIM** 의 개념 및 주요 특징을 설명합니다.

---

## MORAI SIM 이란
MORAI SIM은 자율주행차 개발 및 검증을 위한 시뮬레이션 플랫폼입니다.

MORAI SIM은 자율주행 시뮬레이션의 코어 엔진을 포함한 국내 유일의 풀스택(Full
-stack) 플랫폼으로, VIL(Vehicle-in-the-Loop) 기반의 다양한 주행 테스트 환경을 최신 모빌리티 도메인 사양에 맞추어 제공합니다.

<figure>
<img src="https://static.wixstatic.com/media/f19322_b47ad08287224e28ba1471410aba0172~mv2.jpg" alt="sensor" style="width: 1000px; height: auto;" title="Click to Enlage" onclick="window.open(this.src)">
<figcaption><b> 그림 1. MORAI SIM의 도메인 특화 시뮬레이션 환경</b> 
</figcaption>
</figure>

## MORAI SIM 주요 특징
MORAI SIM은 복잡한 물리적 특성을 반영한 차량 및 센서 모델 뿐만 날씨, 조도, 장애물에 따른 주행 환경을 아니라 디지털 트윈 기술로 구현합니다. 또한 도로에서 재현하기 어려운 검증 환경에 대한 테스트 시나리오를 자동 생성하여 사실적이고 다양한 엣지 및 코너 케이스를 테스트할 수 있습니다.

 MORAI SIM의 주요 특징은 다음과 같습니다.

- **실제 차량 모델**: <Br> 
MORAI SIM은 세단, SUV, 상용차(버스, 트럭)를 비롯하여 항공, 선박, 로봇 분야를 포괄하는 다양한 주행 모델을 지원합니다.
또한 도메인 별 특화 사양과 실제 거동 시험 데이터를 반영하므로 실차 시험과 동일한 조건으로 자율주행 테스트를 할 수 있습니다. 

<figure>
<img src="../img/intro-simdrive3.png" alt="sensor" style="width: 500px; height: auto;" title="Click to Enlage" onclick="window.open(this.src)">
<figcaption><b> 그림 2. MORAI SIM: Drive의 차량 모델</b></figcaption>
</figure>

- **센서 아키텍처**: <Br> 
MORAI SIM의 센서 아키텍처는 다양한 형식의 센서 데이터를 생산 및 실시간 전송합니다. <Br> 따라서 사용자의 필요에 따라 카메라 초점 거리, LiDAR, GPS, IMU 의 노이즈 필터 등 각 센서 파라미터를 자유롭게 조정할 수 있습니다. 또한 다양한 환경 변화(날씨, 조도 등) 및 센서 특성을 반영한 정답 데이터셋을 자동으로 생성할 수 있어 자율주행 인지 모델 학습에 활용할 수 있습니다. 

<figure>
<img src="../img/intro-simdrive4.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)">
<figcaption><b> 그림 3. MORAI SIM의 센서 아키텍처</b> 
</figcaption>
</figure>

- **디지털 트윈 구현 기술**: <Br> 
MORAI SIM은 국내 20여 개의 도시를 비롯한 전세계 주요 도시의 모든 환경 요소를 디지털 트윈으로 구현합니다. <Br> MORAI SIM만의 정밀 지도 데이터 생성 기술을 활용하여 실제와 가상 환경 간의 차이를 최소화한 디지털 트윈 시뮬레이션 환경을 자동 구축합니다.

<figure>
<img src="https://static.wixstatic.com/media/abc373_1cc8ab1566f349da938f5fc3695660d0f000.jpg/v1/fill/w_470,h_360,al_c,q_80,usm_0.33_1.00_0.00,enc_auto/abc373_1cc8ab1566f349da938f5fc3695660d0f000.jpg" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)">
<figcaption><b> 그림 4. MORAI SIM의 디지털 트윈 기반 시뮬레이션 환경</b> 
</figcaption>
</figure>


- **다양한 조건의 테스트 시나리오**: <Br> 
MORAI SIM는 ISO, ASAM, Euro NCAP과 같은 국제 안전 표준에 맞추어 다양한 조건의 테스트 시나리오를 생성합니다. <br>
따라서 실제 데이터셋을 바탕으로 날씨, 차량, 장애물, 궤적과 같은 다양한 주행환경 조건에 대해 사용자 설정에 따라 테스트할 수 있으며 직관적인 그래픽 사용자 인터페이스(GUI) 기반에서 시나리오를 쉽게 편집하고 생성할 수 있습니다.

  <figure>
  <img src="../img/intro-simdrive5.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)">
  <figcaption><b> 그림 5. MORAI SIM에서 생성한 테스트 시나리오</b> 
  </figcaption>
  </figure>


- **클라우드 기반 시뮬레이션 환경**: <Br> 
MORAI SIM는 자체 클라우드 서버를 구축하여 하드웨어 제약 없이 수천 개의 시뮬레이션을 동시에 수행할 수 있습니다. <Br>
MORAI SIM 클라우드 시스템에서는 분산 컴퓨팅을 이용하여 센서 및 차량에 대한 연산 처리를 분배할 수 있어 하여 보다 빠른 시뮬레이션이 가능합니다. 또한 실패한 시나리오에 대한 알고리즘을 클라우드 상에서 수정 및 개선하여 연속적인 시나리오 테스트가 가능합니다.
   <figure>
      <img src="../img/intro-simcloud.png" alt="sensor" style="width: 500px; height: auto;"  title="Click to Enlage" onclick="window.open(this.src)">
      <figcaption><b> 그림 6. MORAI SIM 클라우드 시스템의 시나리오 테스트</b> 
      </figcaption>
    </figure>