<img src="https://github.com/user-attachments/assets/fba52741-1421-4209-9b48-6d65ea4941b4" width="100%" alt="Snow-covered mountain road and tunnel" />

<div align="center">

# Jinsung Kim

### Robotics Systems Software Engineer

**Algorithms → Communication → Hardware → Field Validation**

[![Portfolio](https://img.shields.io/badge/Portfolio-dmdnot.com-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://dmdnot.com)
[![GitHub](https://img.shields.io/badge/GitHub-ranbier-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ranbier)

</div>

## About Me

로봇 알고리즘과 통신 인터페이스, 실제 하드웨어 동작 사이를 연결하고 검증하는 소프트웨어 엔지니어입니다.

- ROS 2 기반 자율주행·수중로봇 시스템 통합
- C/C++ 기반 제어 및 하드웨어 인터페이스 구현
- 로그, 텔레메트리, 오실로스코프와 계측기를 활용한 문제 분리
- 시뮬레이션을 넘어 실제 플랫폼에서 반복 검증

## Featured Work

### 🌊 Autonomous Underwater Vehicle — System Integration

> **2026 Iwakuni Underwater Robot Festival · Senior Division 3rd Place**

- DVL, IMU, Depth 데이터를 결합한 EKF Localization 통합
- Jetson–Pixhawk 간 ROS 2, MAVROS, MAVLink 통신 구성
- YOLO 부표 인식과 자율 미션 상태 전이 연결
- 소프트웨어와 독립적으로 8개 Thruster PWM을 차단하는 Hardware E-Stop 제작
- 센서·알고리즘·추진기·전원을 분리 검증한 뒤 수조에서 통합 테스트

[![AUV Repository](https://img.shields.io/badge/View_AUV_Repository-0077B5?style=flat-square&logo=github&logoColor=white)](https://github.com/2026-kmu-underwater-robot/auv)

### 🚗 ERP-42 Autonomous Driving — Control & System Integration

> **Software Team Lead · Jul 2024–Dec 2025 · 2025 Autonomous Driving Robot Race Grand Excellence Award / 2nd Place**

- Dual u-blox F9P 기반 위치·헤딩 추정과 Localization 구성
- MPC 경로 추종 및 ERP-42 차량 인터페이스 통합
- 실제 차량 응답에 맞춰 MPC 가중치와 명령 발행 주기 튜닝
- GPS covariance가 `0.000196`을 넘으면 속도를 낮추는 degraded operation 구현
- 파라미터를 YAML로 분리해 재빌드 없이 현장 튜닝 가능하도록 개선

[![Waypoint System](https://img.shields.io/badge/Waypoint_System-22C55E?style=flat-square&logo=github&logoColor=white)](https://github.com/ranbier/waypoint_system)
[![Dual GPS Localization](https://img.shields.io/badge/Dual_GPS_Localization-22C55E?style=flat-square&logo=github&logoColor=white)](https://github.com/ranbier/dual_gps_robot_localization)
[![MPC Path Tracking](https://img.shields.io/badge/MPC_Path_Tracking-22C55E?style=flat-square&logo=github&logoColor=white)](https://github.com/ranbier/mpc_pathtracking)

### ⚡ 1/5 Scale EV — Digital-to-Analog Control Interface

> **Autonomous Driving Competition Encouragement Award**

- Arduino PWM을 RC Low-pass Filter를 통해 HENES T580용 아날로그 입력으로 변환
- Steering 입력 전압 범위를 멀티미터로 측정
- PWM 및 필터 출력 파형을 오실로스코프로 검증
- 수동·자율 주행 코스 테스트를 반복해 조향 및 구동 실패 없이 완주

### 🔧 MPC5604P — Register-Level Motor Control

- GPIO, ADC, FlexPWM, eTimer를 레지스터 레벨에서 구성
- Motor current PI 제어와 Encoder 기반 speed control 구현
- 과열·과전압·단락 상황에서 PWM을 차단하는 protection logic 구현
- FreeMaster와 오실로스코프로 전압·전류·속도 응답 검증

## Publications

- **First Author** — *A Real-Time Optimal Avoidance Path Generation Method for MPC-Based Autonomous Vehicles*, KSAE Spring Conference 2025
- **Co-Author** — *Nonlinear MPC Path Tracking with Variable Steering-Angle Weights*, KSAE Spring Conference 2025
- **Co-Author** — *Sequential Multi-Critic PPO and Critic Transfer for Autonomous Lane Following*, KSAE Fall Conference 2025

## Tech Stack

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![ROS 2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![NVIDIA](https://img.shields.io/badge/Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)

`ROS 2` · `MAVROS` · `MAVLink` · `CAN` · `EKF` · `MPC` · `YOLO` · `Embedded C`

## GitHub

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=ranbier&show_icons=true&hide_border=true&theme=transparent&rank_icon=github)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=ranbier&layout=compact&hide_border=true&theme=transparent)

</div>

---

<div align="center">
실제 로봇의 동작으로 검증되는 소프트웨어를 만듭니다.
</div>
