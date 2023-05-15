# 시스템 요구사항
 **MORAI SIM** 실행에 앞서 필요한 시스템 사양 및 구성, 라이선스에 대해 설명합니다.

---

## 시스템 사양
**MORAI SIM** 을 실행하는 시스템의 사양은 기본 사양과 추천 사양으로 구분합니다.

### 기본 사양
MORAI SIM을 실행하기 위한 최소 기본 사양은 아래와 같습니다.
>
- **CPU**: Intel i5-9600KF or AMD Ryzen 5 3500X
- **RAM**: DDR4 16GB
- **VGA**: NVIDIA GeForce RTX 2060 Super

### 추천 사양
MORAI SIM에서 다수의 카메라 및 라이다 센서를 사용할 경우, 추천 시스템 사양은 아래와 같습니다.
> 
- CPU: Intel i7 or higher
- RAM: 32GB  or higher
- VGA: RTX 30 series or higher

###  운영체제 사양
>
- Windows: 10 or higher
- Linux: Ubuntu 18.04 LTS or higher

## 시스템 구성
MORAI SIM을 실행하는 시스템 구성 방식 및 각 시스템에서 사용하는 통신은 아래와 같습니다.

### 단일 시스템
자율주행 로직과 시뮬레이터가 동일 시스템에서 실행하는 방식입니다. <Br>
단일 시스템 내에서 자율주행 로직과 시뮬레이터 간 통신으로 ROS, UDP를 사용합니다.
![Image title](../img/getting-singlesystem.png){:onclick="window.open(this.src)" title="Click view screen"}

### 멀티 시스템
자율주행 로직과 시뮬레이터가 서로 다른 시스템에서 실행하는 방식입니다. <Br>
각 시스템은 Ethernet 또는 Wi-Fi로 연결되며, 자율주행 로직과 시뮬레이터 간 통신으로 ROS, UDP를 사용합니다.
![Image title](../img/getting-multisystem.png){:onclick="window.open(this.src)" title="Click view screen"}

???+ warning
    ROS 통신의 경우, 리눅스 운영체제 시스템에서만 동작하므로 ROS 통신으로, 단일 시스템 혹은 멀티 시스템 내에 시뮬레이터를 제어하는 자율주행 로직은 우분투 운영체제에서 실행해야 합니다.

## 라이선스
시뮬레이터를 실행하려면 사용자 시뮬레이터 제품에 맞는 유효한 라이선스가 필요합니다.
???+ note
    라이선스 구매 관련하여 [모라이 담당 부서](https://moraisim.typeform.com/to/RrF9RIFl){:target="_blank"}에 문의하여 주십시오.

라이선스를 활성화하기 위해 필요한 사항은 아래와 같습니다. 

- 인터넷 환경: 시뮬레이터 런처를 다운받아 사용자 계정으로 런처에 로그인하기 위함
- 사용자 계정(ID/PW): [모라이 라이선스 센터](https://dev-admin.morai-sim.com/#/sign){:target="_blank"}에 등록된 사용자 계정(ID/PW)으로 런처에 로그인 후 시뮬레이터를 설치 및 실행함

???+ note 
    2020년 이후 공식 시뮬레이터 버전부터는 사용자 계정의 라이선스 활성화 방식만 지원합니다. <br>
    단, 인터넷을 사용할 수 없는 환경인 경우, USB 동글을 이용하여 라이선스 활성화 및 시뮬레이터를 설치할 수 있습니다. 관련한 자세한 사항은 모라이 프로젝트 담당자에게 문의하십시오.


