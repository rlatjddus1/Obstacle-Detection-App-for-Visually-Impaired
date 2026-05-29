
# 🦯 보행자 감지 및 사고 예방을 위한 개인 이동형 보조 시스템

> 시각장애인 및 교통 약자를 위한 AI 기반 실시간 위험 감지 시스템
> SW 창업 아이디어 경진대회 출품 프로젝트

---

# 📌 Overview

본 프로젝트는 시각장애인과 교통 약자의 안전한 보행을 지원하기 위해
실시간 객체 탐지, 객체 추적, 깊이 추정 기술을 결합한
AI 기반 보행 안전 보조 시스템입니다.

개인 이동형 장비(지팡이, 휴대 장치 등)에 탑재 가능한 형태를 목표로 하였으며,
보행 중 주변 위험 객체를 탐지하고 음성으로 안내하여
사고를 예방할 수 있는 시스템을 설계했습니다.

---

# 📅 Project Information

| Category     | Content                          |
| ------------ | -------------------------------- |
| Project Name | 보행자 감지 및 사고 예방을 위한 개인 이동형 보조 시스템 |
| Period       | 2024.12.07 ~ 2024.12.20          |
| Team         | 박진성, 김성연, 김남규                    |
| Goal         | AI 기반 실시간 보행 안전 보조 시스템 개발        |

---

# 🛠 Tech Stack

## AI / Vision

* YOLOv8
* MiDaS
* OpenCV
* PyTorch

## Mobile / Backend

* React Native
* Node.js
* Socket Programming

## Additional

* TTS (Text-to-Speech)
* Kalman Filter

---

# 🎯 Development Goal

* 시각장애인 및 교통 약자를 위한 실시간 위험 감지 시스템 개발
* 이동형 장비 기반 보행 보조 서비스 설계
* 객체 탐지 + 객체 추적 + 깊이 추정을 결합한 위험 분석 시스템 구현
* 음성 안내 기반 사용자 친화적 인터페이스 제공

---

# ⚙️ System Features

## 👀 실시간 객체 탐지

YOLOv8 모델을 활용하여 보행 환경 내 다양한 객체를 탐지했습니다.

### Detection Target

* 보행자
* 자전거
* 오토바이
* 킥보드
* 기타 이동체

---

## 🎯 객체 추적 시스템

칼만 필터(Kalman Filter)를 적용하여
실시간 영상 내 객체 이동 경로를 추적했습니다.

이를 통해 단순 탐지를 넘어
연속적인 위험 상황 분석이 가능하도록 구현했습니다.

---

## 📏 깊이 추정 기반 거리 분석

MiDaS 모델을 활용하여 객체와 사용자 간 상대 거리를 추정했습니다.

깊이 정보를 기반으로 위험 객체 접근 여부를 판단하여
충돌 가능성을 분석할 수 있도록 설계했습니다.

<img width="600" height="250" alt="미다스적용사진" src="https://github.com/user-attachments/assets/d5d5f474-5212-490b-8d56-1e239f41588d" />

---


## 🔊 음성 안내 시스템

TTS(Text-to-Speech)를 활용하여
위험 상황 발생 시 사용자에게 음성으로 경고를 제공했습니다.

예시:

* "왼쪽에서 자전거가 접근 중입니다."
* "전방에 보행자가 있습니다."

---

## 🌐 서버–클라이언트 구조

Socket Programming 기반 통신 구조를 설계하여
모바일 애플리케이션과 AI 처리 서버 간 데이터를 송수신했습니다.

또한 로그 관리 시스템을 구현하여
위험 감지 이벤트를 기록 및 관리할 수 있도록 구성했습니다.

<img width="664" height="498" alt="보행자 보조 시스템_시퀀스다이어그램" src="https://github.com/user-attachments/assets/f819845c-08eb-4eba-9aaf-ec4d51e03e8d" />

---

# 📱 Application Workflow

1. Node.js 기반 서버 실행 (`server.js`)
2. React Native 앱 실행 (`App.tsx`)
3. Start Capture 버튼 클릭
4. Python 기반 AI 서버 실행 (`app.py`)
5. 실시간 위험 감지 및 음성 안내 수행

---

# 🧪 Tech Highlights

* YOLOv8 기반 실시간 객체 탐지
* Kalman Filter 기반 객체 추적
* MiDaS 기반 Depth Estimation 적용
* 실시간 카메라 영상 처리
* TTS 기반 음성 피드백 시스템
* Socket 기반 서버–클라이언트 통신 구조 설계

---

# 🏆 Achievement

* SW 창업 아이디어 경진대회 출품
* AI 기반 보행 안전 보조 시스템 실현 가능성 검증
* 휴대형 AI 보조 장치 아이디어 제안

---

# 📚 What I Learned

* 객체 탐지 + 객체 추적 + 깊이 추정 융합 처리 경험
* 실시간 영상 처리 시스템 설계 경험
* React Native 기반 모바일 연동 경험
* Socket 통신 기반 시스템 구조 설계 경험
* 사회적 약자를 위한 AI 서비스 설계 경험

---

# ⚡ Version

| Component             | Version |
| --------------------- | ------- |
| React Native          | 0.76    |
| Metro                 | 0.81.0  |
| Android Gradle Plugin | 8.6.0   |
| Gradle                | 8.10.2  |
| Python                | 3.12.7  |
| Node.js               | 20.11.1 |
