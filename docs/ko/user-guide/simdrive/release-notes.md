# Release Notes
MORAI SIM: Drive에 반영된 추가 및 개선 사항, 오류 수정 사항을 최신 및 지난 배포 버전 별로 설명합니다.

---

## Latest

|  Version        | Release Date | Additions and Changes   | Bug Fixes   | 
| --------------- | :----------- | ----------------------- | ----------- |
|  22.R4.2        | 2023/04/14   | N/A                     | [1건](#bug-fixes) |

<br>

### Additions and Improvements

??? Info "해당 없음"

<br>
### Bug Fixes

??? bug "Ego Vehicle 정지 오류"

    - 2016_Hyundai_Ioniq Ego 차량을 ROS Ego Ctrl Cmd 로 제어 중 acceleration -1 m/s^2 로 Publish 시 정상적으로 정지 불가 오류 해결
        - 해당 제어 명령에서 정상적으로 속도가 감소 후 정지함
        ![Image title](../img/rel-bug1.png){:onclick="window.open(this.src)" title="Click view screen"}

<br>

## Previous versions