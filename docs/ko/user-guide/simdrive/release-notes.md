# 릴리스 노트
MORAI SIM: Drive에 반영된 변경 및 개선 사항, 오류 수정 사항을 최신 및 지난 배포 버전 별로 설명합니다.

---

## 최신 버전

|  Version        | Release Date | Additions and Changes   | Bug Fixes   | 
| --------------- | :----------- | ----------------------- | ----------- |
|  22.R4.2        | 2023/04/14   | N/A                     | [1건](#bug-fixes) |

<br>

### 변경 및 개선 사항

??? Info "해당 없음"

<br>
### 오류 수정 사항

??? bug "Ego Vehicle 정지 오류"
    - 2016_Hyundai_Ioniq Ego 차량을 ROS Ego Ctrl Cmd 로 제어 중 acceleration -1 m/s^2 로 Publish 시 정상적으로 정지 불가 오류 수정
        - 해당 제어 명령에서 정상적으로 속도가 감소 후 정지함
        ![Image title](../img/rel-bug1.png){:onclick="window.open(this.src)" title="Click view screen"}

??? bug " 런처 창크기 활성화 오류"
    - MORAI SIM 런처의 창 크기가 작을 때 크기 조절 드래그 커서가 활성화되지 않는 오류 수정
    ![Image title](../img/rel-bug2.png){:onclick="window.open(this.src)" title="Click view screen"}

??? bug "맵 진입 불가 오류"
    - **R_KR_PR_GWJmap** 맵 진입 불가 오류 수정
    - Ubuntu 20.04 OS 환경에서 **R_KR_PR_SejongBRT0** 맵 진입 불가 오류 수정

??? bug "객체 삭제 불가 오류"
    - 특정 차량 객체, **OBJ_Hyundai_Xcient_P520** 배치 후 삭제 불가 오류 수정
    ![Image title](../img/rel-bug3.png){:onclick="window.open(this.src)" title="Click view screen"}
<br>


## 지난 버전
지난 버전에 대한 변경 이력은 이전 기술 문서 사이트의 [릴리스 노트](https://help-morai-sim.scrollhelp.site/morai-sim-standard-kr/release-notes){:target="_blank"}를 참고하십시오.