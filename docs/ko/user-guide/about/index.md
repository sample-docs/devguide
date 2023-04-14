# 본 문서에 관하여
This section describes the purpose, target audiences, and scope of this document.

---

## 문서 개요

### Purpose
This document is written to guide the configuration environment and usage of ‘MORAI SIM: Air’, an autonomous flight simulation platform developed by Morai.

### Target Audience
This document is written for aeronautical developers and researchers who want to verify air vehicles in various simulated virtual environments.

### Scope
The scope of application of this document applies to the configuration environment and user interface of MORAI SIM: Air, and all functions provided by MORAI SIM: Air.

## 문서 개정 이력
This section describes the revision history of the document in chronological order.

| Document Version | Product Version | Release Date  | Descriptions             | Author  |
| :--------------- | :---------------| :------------ | :----------------------- | :------ |
| 1.0              | Alpha 1.0            | April 4, 2023   | Initial Release   | MORAI Engineering Service Team |


## 용어 및 약어
The key Terms and Abbreviations used in this documents are listed below:

| Terms and Abbreviations | Descriptions                           |
| ----------------------- | -------------------------------------- |
| Ego Vehicle             | Control flight target aircraft in the simulator |
| NPC Vehicle             | Surrounding aircraft that are not controlled flight targets in the simulator |
| ROS2                    | The latest version of Robot Operating System(ROS) |
| JSBSim                  | An open source, multi-platform, object-oriented flight dynamics model (FDM) framework written in the C++ programming language |
| AOA                     | Angle of Attack, unit: degrees                     |
| CAS                     | Calibrated Airspeed, unit: knots            |
| GS                      | Ground Speed, unit: knots                |
| Attitude Indicator      | Shows the altitude of the aircrafte                       |
| Altimeter               | Shows the altitude of the aircraft above ground level(AGL) in feet                        |
| Vertical Speed Indicator | Shows the vertical speed of the aircraft in feet per minute                      |


## 표기 규칙
The notational conventions for notes, warnings, and tips used in this document are as follows:

<div markdown="span" class="bs-callout bs-callout-primary">
ℹ️ <span class = "not-calloutTitle"> NOTE </span> <br>
General Information for related matters.
</div>
<p></p>
<div markdown="span" class="bs-callout bs-callout-danger">
⚠️  <span class = "dan-calloutTitle"> WARNING </span> <br>
For matters you should follow when setting or configuration
</div>
<p></p>
<div markdown="span" class="bs-callout bs-callout-success">
✅ <span class = "suc-calloutTitle"> TIPS </span> <br>
Useful tips when setting or configuration
</div>

<br>
