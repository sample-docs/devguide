# 기본 화면 UI
t시뮬레이터를 실행하면 나타나는 기본 화면 UI의 구성 요소에 대해 설명합니다.

---

## 기본 화면 UI 개요
The default UI appears as soon as you enter the simulater for the first time. <br>
Centered on the map and aircraft selected in the previous step, it consists of the following three parts: **1] Network and Sensor Settings**, **2] Environment Settings**, and **3] Flight Instruments**.
<figure>
  <img src="../../img/ui-default2.png" alt="sensor" style="width: 1000px; height: auto;" title="Click to Enlage" onclick="window.open(this.src)">
  <figcaption style="padding-top: 10px;"><b> Figure 2. Default UI of MORAI SIM: Air</b> 
  </figcaption>
</figure>

### 1] Network and Sensor Settings
This menu is located in the upper left menu of the simulator screen, and provides access to the  network and sensor settings, which are the core features provided by the simulator.
<img src="../../img/ui-netsen.png" alt="launcher">

<div markdown="span" class="bs-callout bs-callout-success">
✅ <span class = "suc-calloutTitle"> TIPS </span> <br>
For details on how to use network and sensor functions, see the <a href="../../user-guide/">Using MORAI SIM: AIR</a> part.
</div>

### 2] Environment Settings
This menu is located in the upper right menu of the simulator screen, and provides weather and time of day configurations that determine the background and lighting of the simulator.
<img src="../../img/ui-env.png" style="width: 500px; height: auto;" alt="launcher">

## Aircraft Info UI
The **Aircraft Information** UI provides the aircraft control mode and current flight status such as airspeed and air pressure, as well as steering inputs for control surfaces and attitude, in detailed numerical values.

If you click the mouse on the **Ego aircraft**, the Aircraft Information window appears on the right side of the simulator screen as shown below.
<figure>
    <img src="../../img/ui-info.png" alt="info" style="width: 1000px; height: auto;" title="Click to Enlage" onclick="window.open(this.src)">
    <figcaption style="padding-top: 10px;"><b> Figure 3. Aircraft Info UI of MORAI SIM: Air</b></figcaption>
</figure>


### 1] Aircraft Control Mode
Displays the mode to control the Ego aircraft with **Manual Control Mode** and **Network Control Mode**.
<img src="../../img/ui-controlmode.png" style="width: 450px; height: auto;" alt="launcher">

**Manual Control Mode** is a mode in which the user controls the aircraft with a keyboard or joystick. <Br>
The default **Manual Control Mode** is keyboard control, and the keyboard `Q` key toggles between keyboard control and joystick control.
<br>

To control the aircraft with a joystick, connect the joystick to the simulator via USB and press `Q`. Then, to control the aircraft with the keyboard, press `Q` again.

### 2] Propulsion
Displays engine RPM, air speed (knots), thrust according to throttle control and manifold pressure (inHg) according to  aircraft altitude.
<img src="../../img/ui-propulsion.png" style="width: 450px; height: auto;" alt="launcher">

<div markdown="span" class="bs-callout bs-callout-success">
✅ <span class = "suc-calloutTitle"> TIPS </span> <br>
In <b>Manual Control Mode</b>, when you press <code>E</code> on the keyboard, the value of <b>Throttle</b> (up to 1) increases. <br>
In addition, see the <a href="../../user-guide/basic-controls">Basic Controls</a> section for a detailed description of each key used to operate the aircraft with the keyboard in <b>Manual Control Mode.</b>
</div>

### 3] Flight Control
Displays the flight control surfaces and trim control value, as **Primary Control**, along with the **Attitude**, **Vertical Info** and **Airspeed** values ​​of the aircraft in detailed numerical values.
<img src="../../img/ui-flightst.png" style="width: 450px; height: auto;" alt="launcher">


See below for descriptions of abbreviations and terms in **Flight Control**.

<div markdown="span" class="bs-callout bs-callout-primary">
ℹ️ <span class = "not-calloutTitle"> NOTE </span> <br>
  <ul> 
    <li>
    AOA: Angle of Attack (degrees)
    </li>
    <li>
    EAS: Equivalent Airspeed (knots)
    </li>
    <li>
    TAS: True Airspeed (knots)
    </li>
    <li>
    GS: Ground Speed (knots)
    </li>
    <li>
    Climb Rate: Vertical Speed Indicator (feet per minute)
    </li>
    <li>
    Trim: Shows the input data of each trim from -1 to +1
    </li>
  </ul> 
</div>


<div markdown="span" class="bs-callout bs-callout-success">
✅ <span class = "suc-calloutTitle"> TIPS </span> <br>
See the <a href="../../user-guide/basic-controls">Basic Controls</a> section for a detailed description of each key for controlling the flight control surfaces and trim of each Aileron, Elevator, Rudder as <b>Primary Control</b> and Flap as <B>Secondary Control</b>.
</div>
