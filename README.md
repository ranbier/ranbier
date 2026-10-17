<img src="https://github.com/user-attachments/assets/fba52741-1421-4209-9b48-6d65ea4941b4" width="100%" alt="Snow-covered mountain road and tunnel" />

<div align="center">

# Jinsung Kim

### Robotics Systems Software Engineer

**Algorithms → Communication → Hardware → Field Validation**

[![Portfolio](https://img.shields.io/badge/Portfolio-dmdnot.com-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://dmdnot.com)
[![GitHub](https://img.shields.io/badge/GitHub-ranbier-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ranbier)
[![Email](https://img.shields.io/badge/Email-kimss6240%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kimss6240@gmail.com)

</div>

## About Me

로봇의 위치 추정과 경로 추종 알고리즘을 실제 하드웨어·통신 시스템에 연결하고, 실차와 수중 환경에서 검증하는 소프트웨어 엔지니어입니다.

- ROS / ROS 2 기반 자율주행·수중로봇 시스템 통합
- 위성항법·관성 센서·휠 엔코더·수중 속도 센서를 활용한 센서 융합과 위치 추정
- Pure Pursuit 및 모델 예측 제어(Model Predictive Control, MPC) 기반 경로 추종과 실차 튜닝
- C/C++ 기반 제어·하드웨어 인터페이스 구현 및 로그·계측기를 활용한 반복 검증

국민대학교 자동차IT융합학과 · 2027.02 졸업 예정 · 학점 4.23 / 4.5

## Featured Work

### 🌊 Autonomous Underwater Vehicle — System Integration

> **Iwakuni Ocean Tech Days 2026 · Senior Division 3rd Place**
>
> **Jan–Aug 2026 · ROS 2 Sensor & Control System Integration / Underwater Localization**

- 도플러 속도 센서(Doppler Velocity Log, DVL)·관성 측정 장치(Inertial Measurement Unit, IMU)·수심 센서 데이터를 확장 칼만 필터(Extended Kalman Filter, EKF)로 융합해 수중 위치·자세 추정
- Jetson–Pixhawk 간 ROS 2, MAVROS, MAVLink 통신을 구성하고 추정 결과를 제어 시스템과 연계
- YOLO 부표 인식과 자율 미션 상태 전이 연결
- 소프트웨어와 독립적으로 8개 추진기의 펄스 폭 변조(Pulse Width Modulation, PWM) 신호를 차단하는 하드웨어 비상 정지 장치 제작
- 실제 수영장에서 센서 데이터·추정 궤적·제어 동작을 반복 검증

[![Underwater Robotics Team](https://img.shields.io/badge/View_Underwater_Robotics_Team-0077B5?style=flat-square&logo=github&logoColor=white)](https://github.com/2026-kmu-underwater-robot)

### 🚗 ERP-42 Autonomous Driving — Control & System Integration

> **2025 자율주행 로봇레이스 1차 대회 최우수상**
>
> **Jan–Jul 2025 · Localization & Path Tracking Control**

- 보정정보를 수신하는 정밀 위성항법(Real-Time Kinematic Global Navigation Satellite System, RTK-GNSS)과 IMU 기반 위치·진행 방향 추정
- IMU 사용이 제한된 대회에서는 Dual GNSS를 활용해 진행 방향 추정
- Pure Pursuit의 Look-ahead Distance와 MPC 비용함수·제약조건을 차량 속도·경로 곡률·실차 응답에 맞춰 튜닝
- 반복 실차 주행으로 조향 오버슈트와 경로 이탈을 줄이고 ERP-42 차량 인터페이스와 통합
- 파라미터를 YAML로 분리해 재빌드 없이 현장 튜닝 가능하도록 개선

[![Waypoint System](https://img.shields.io/badge/Waypoint_System-22C55E?style=flat-square&logo=github&logoColor=white)](https://github.com/ranbier/waypoint_system)
[![Dual GPS Localization](https://img.shields.io/badge/Dual_GPS_Localization-22C55E?style=flat-square&logo=github&logoColor=white)](https://github.com/ranbier/dual_gps_robot_localization)
[![MPC Path Tracking](https://img.shields.io/badge/MPC_Path_Tracking-22C55E?style=flat-square&logo=github&logoColor=white)](https://github.com/ranbier/mpc_pathtracking)

### 🏎️ Indoor 1/10 Scale Vehicle — Localization & Path Tracking

> **Aug–Oct 2024 · Dead Reckoning Localization & Path Tracking Control**

- 위성항법을 사용할 수 없는 실내에서 휠 엔코더 기반 이동거리·속도와 IMU 기반 회전 상태 추정
- `robot_localization`의 EKF로 센서 데이터를 융합해 초기 위치 기준의 상대 위치·자세를 추정하는 추측 항법(Dead Reckoning) 구성
- 실차 데이터로 프로세스 잡음 공분산(Process Noise Covariance)을 튜닝해 추정 안정성 개선
- 추정 궤적으로 실내 주행용 경유점(Waypoint) 경로를 생성하고 Pure Pursuit 경로 추종 구현

### ⚡ 1/5 Scale EV — Digital-to-Analog Control Interface

> **HL FMA (Future Mobility Award) 2025 자율주행 경진대회 장려상 · aMAP Innovator Championship [1/5] 부문**

- Arduino PWM 신호를 저항·커패시터 기반 저역 통과 필터로 변환해 HENES T580용 아날로그 제어 입력 생성
- Steering 입력 전압 범위를 멀티미터로 측정
- PWM 및 필터 출력 파형을 오실로스코프로 검증
- 수동·자율 주행 코스 테스트를 반복해 조향 및 구동 실패 없이 완주

### 🔧 MPC5604P — Register-Level Motor Control

> **Sep–Dec 2025 · Motor Control Logic / Peripheral Configuration**

- GPIO, ADC, FlexPWM, eTimer를 레지스터 레벨에서 구성
- 엔코더 기반 속도 피드백과 아날로그-디지털 변환기(Analog-to-Digital Converter, ADC) 기반 전류 피드백 구성
- 속도 비례·적분 제어기(Proportional-Integral Controller, PI)의 출력으로 목표 전류를 생성하고, 전류 PI 제어기로 PWM 듀티를 계산하는 직렬 제어(Cascade Control) 구현
- 타이머 인터럽트로 일정한 제어 주기를 구성하고 H-Bridge 구동 신호 생성
- 과열·과전압·단락 상황에서 PWM을 차단하는 보호 로직 구현
- FreeMaster와 오실로스코프로 실제 모터의 전압·전류·속도 응답 검증

## Publications

- **제1저자** — *MPC 기반 자율주행 차량의 실시간 최적 회피 경로 생성 방법론*, 2025 한국자동차공학회 춘계학술대회
- **제2저자** — *Arctangent 함수를 활용한 가변 조향각 변화량 가중치 기반 비선형 모델 예측 제어의 경로 추종 성능 및 주행 안정성 향상 연구*, 2025 한국자동차공학회 춘계학술대회
- **Co-Author** — *Sequential Multi-Critic PPO and Critic Transfer for Autonomous Lane Following*, KSAE Fall Conference 2025

## Tech Stack

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![ROS](https://img.shields.io/badge/ROS-22314E?style=flat-square&logo=ros&logoColor=white)
![ROS 2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![NVIDIA](https://img.shields.io/badge/Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)

`ROS / ROS 2` · `MAVROS / MAVLink / ArduSub` · `Pure Pursuit / MPC` · `EKF / Sensor Fusion` · `GNSS / IMU / DVL` · `Embedded C`

## GitHub

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=ranbier&show_icons=true&hide_border=true&theme=transparent&rank_icon=github)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=ranbier&layout=compact&hide_border=true&theme=transparent)

</div>

---

<div align="center">
문제를 마주하고, 해결될 때까지 끝까지 파고듭니다.<br>
실제 로봇의 동작으로 검증되는 소프트웨어를 만듭니다.
</div>
