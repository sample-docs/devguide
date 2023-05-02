# 기본 화면 UI
시뮬레이터를 실행 시 초기 화면으로 보여주는 **기본 화면 UI** 에 대해 설명합니다.

---

## 기본 화면 UI 구성
시뮬레이터를 실행하면 나타나는 기본 화면 UI의 구성은 아래와 같습니다.
![uidefault](../../img/simdrive-ui-default.png){:onclick="window.open(this.src)" title="Click view screen"}
<figcaption><center><b> 그림 1. MORAI SIM: Drive 기본 화면 UI 구성</b></center></figcaption>
<br>
시뮬레이터 기본 화면 UI는 시뮬레이터 실행 시 선택한 맵과 차량의 배경을 중심으로 화면 상단의 **1] 툴바**, 하단의 **2] 상태바**, 시뮬레이터 화면 상단 좌우의 **3] 화면 영역 및 카메라 설정**, **4] 환경 설정** 메뉴로 구성됩니다.


## 1] 툴바
센서 및 시나리오 구성, 외부 시스템 간 데이터 전송을 위한 네트워크 설정 등 시뮬레이터에서 제공하는 주요 기능에 접근합니다.

툴바의 세부 메뉴 항목은 아래와 같습니다.

- **Edit**: 맵 및 차량 선택, 센서 및 시나리오 구성, 네트워크 설정 등 시뮬레이터의 주요 기능 메뉴
- **View**: 현재 차량에서 사용 중인 센서, 네트워크, 장애물에 대한 리스트 보기 메뉴
- **PlayMode**: Rosbag 및 Network Replay 등 시뮬레이터의 고급 기능 메뉴
- **Tools**: 시뮬레이터 시스템 및 그래픽 조정 옵션 메뉴
- **Help**: 시뮬레이터 단축키 및 시스템 정보 메뉴
- **Time Manager**: 시뮬레이터 동작 주기 설정 메뉴
- **Recording mode**: 시뮬레이션 화면을 녹화하는 경우, 주행 차량을 제외한 화면 내 모든 UI 요소 숨기기 메뉴(툴바 맨 우측에 위치).
    ![uidefault](../../img/simdrive-ui-recording.png){:onclick="window.open(this.src)" title="Click view screen"}
    <figcaption><center><b> 그림 2. Recording mode 활성화 화면</b></center></figcaption>

    ???+ tip
         **Recording mode** 는 시뮬레이션 화면을 녹화하는 기능이 아닙니다. MORAI SIM은 녹화 기능을 제공하지 않으므로, 녹화가 필요한 경우 별도의 동영상 프로그램을 사용하십시오. 

## 2] 상태바
실행 중인 시뮬레이터에 대한 아래 정보를 확인합니다.

- 버전명
- 라이선스 계정명(**Username**)
- 실행 상태 로그 보기(**+**)

    ???+ tip
        시뮬레이터 하단 상태바의 맨 우측에서 **+** (단축키 `)를 클릭하면 현재 실행 중인 시뮬레이터의 상태 로그를 정보, 경고, 오류 수준별로 확인할 수 있습니다.
        ![uidefault](../../img/simdrive-ui-log.png){:onclick="window.open(this.src)" title="Click view screen"}

## 3] 화면 영역 및 카메라 설정
시뮬레이터의 화면 영역(Viewport)과 화면 보기 카메라(Camera)를 설정합니다.

  - **Viewport Setting**: 시뮬레이터 화면 상단 좌측의 **톱니바퀴**(**⚙️**) 버튼을 클릭하면 아래와 같이 화면 영역에 보여지는 메뉴를 선택할 수 있습니다.

    ![uidefault](../../img/simdrive-ui-viewport.png){:onclick="window.open(this.src)" title="Click view screen" width="300px"}

    ???+ tip
        시뮬레이터 실행 시 화면에 기본으로 보여지는 항목은 Ego 차량에 대한 **Vehicle Label** 입니다. 예를 들어, Ego 차량이 한 대이면 해당 Ego 차량 위에 'Ego-0'로 표시됩니다.

<br>

  - **Camera Setting**: 시뮬레이터 화면 상단 좌측의 **카메라**(**🎥**) 버튼을 클릭하면 시뮬레이터 화면을 보여주는 카메라 시점 및 카메라 성능을 설정할 수 있습니다. 

    ![uidefault](../../img/simdrive-ui-camera.png){:onclick="window.open(this.src)" title="Click view screen" width="300px"}
<br>

## 4] 환경 설정
시뮬레이터 주행 환경에 대한 시간대와 날씨를 설정합니다. 
 
  - **Time**: 시뮬레이터 화면 상단 우측의 **Time**(**🕓**) 버튼을 클릭하면 아래와 같이 화면 조도를 결정하는 시간대를 선택할 수 있습니다.
  
    ![uidefault](../../img/simdrive-ui-time.png){:onclick="window.open(this.src)" title="Click view screen" width="300px"}
<Br>

  - **Weather**: 시뮬레이터 화면 상단 우측의 **Weather**(**☁️**) 버튼을 클릭하면 아래와 같이 눈, 비, 안개와 같은 날씨 효과를 선택할 수 있습니다.
  
    ![uidefault](../../img/simdrive-ui-weather.png){:onclick="window.open(this.src)" title="Click view screen" width="300px"}

    ???+ tip
        Weather 항목 중 **Rainy** 를 선택하면 실제 빗소리를 포함하여 비오는 날씨의 주행 환경을 재현할 수 있습니다.

        ![uidefault](../../img/simdrive-ui-rain.png){:onclick="window.open(this.src)" title="Click view screen" width="300px"}


