# 🏢 SmartSpend (AI 기반 RPA 사내 협업 시스템)

> **단순 정보 제공이 아닌, AI가 실제 업무를 자동 처리하는 차세대 협업 플랫폼**

## 1. 📅 프로젝트 개요

- **프로젝트명**: SmartSpend
- **개발 기간**: 2025.12.15 ~ 2026.01.16 (약 5주)
- **프로젝트 소개**:
  `SmartSpend`는 기업 내 반복되는 업무(경비 처리, 출결, 결재 등)로 인한 생산성 저하를 해결하기 위해 기획되었습니다. 기존 ERP의 수동 작업 한계를 넘어, **AI 챗봇과 RPA(Robotic Process Automation)** 기술을 도입하여 자연어 명령만으로 업무를 자동 처리하고, OCR 및 얼굴 인식을 통해 사용자 편의성을 극대화한 사내 협업 시스템입니다.

## 2. 👥 팀원 소개 (Team 1)

| <a href="http://github.com/haechan419"><img src="https://github.com/haechan419.png" width="100px" alt="한해찬"/><br /><sub><b>한해찬 (팀장)</b></sub></a> | <a href="https://github.com/shanekang1"><img src="https://github.com/shanekang1.png" width="100px" alt="강진수"/><br /><sub><b>강진수</b></sub></a> | <a href="https://github.com/Moonjooyeon"><img src="https://github.com/Moonjooyeon.png" width="100px" alt="문주연"/><br /><sub><b>문주연</b></sub></a> | <a href="https://github.com/parucho-1358"><img src="https://github.com/parucho-1358.png" width="100px" alt="성건우"/><br /><sub><b>성건우</b></sub></a> | <a href="https://github.com/ujyj0414-dotcom"><img src="https://github.com/ujyj0414-dotcom.png" width="100px" alt="전유진"/><br /><sub><b>전유진</b></sub></a> |
| :---: | :---: | :---: | :---: | :---: |


<br>

### 📝 역할 분담 (R&R)

* **한해찬 (팀장)**
    * 프로젝트 총괄 및 통합, 코드 리팩토링
    * AI(Ollama)를 이용한 Todo 자동화(CRUD) 구현
    * 메인 화면 반응형 웹 구현 및 파일 업로드 처리

* **강진수**
    * 전체 Layout 구현 및 알림 기능 개발
    * 비품 페이지 및 승인/신청 기능 구현(CRUD) , 장바구니 기능(CRUD)
    * face-api.js를 활용한 얼굴 인식 로그인 구현

* **문주연**
    * 업무 보드 및 실시간 채팅(개인/그룹) 구현
    * 채팅 내 파일 업로드/다운로드 및 채팅 AI 챗봇 연동
    * 전체 DB 설계 및 프로젝트 일정 관리

* **성건우**
    * Spring Security + JWT 기반 로그인/인증 구현
    * 사원 관리 페이지 및 마이페이지, 근태(출결) 관리 기능
    * 사원 관련 AI 챗봇 구현, 회의록 및 진행 일지 작성

* **전유진**
    * 영수증 OCR 기능 구현 (이미지 텍스트 추출)
    * 지출 결재 관리 시스템 및 회계 통계 시각화
    * 전체 프로젝트 플로우 차트 통합 제작

      
## 3. 🛠️ 기술 스택 (Tech Stack)

### **Back-End** &nbsp; <img src="https://img.shields.io/badge/-ED8B00?style=flat-square&logo=openjdk&logoColor=white"> <img src="https://img.shields.io/badge/-6DB33F?style=flat-square&logo=springboot&logoColor=white"> <img src="https://img.shields.io/badge/-3776AB?style=flat-square&logo=python&logoColor=white"> <img src="https://img.shields.io/badge/-009688?style=flat-square&logo=fastapi&logoColor=white">
- **Language**: Java, Python
- **Framework**: Spring Boot, FastAPI
- **Security**: Spring Security, JWT
- **Data/Network**: Spring Data JPA, Spring WebSocket (STOMP/SockJS), Spring Data Redis
- **Library**: Apache POI, OpenPDF, Thumbnailator, ModelMapper, Jackson Databind, Gson, OkHttp

### **Front-End** &nbsp; <img src="https://img.shields.io/badge/-F7DF1E?style=flat-square&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/-20232A?style=flat-square&logo=react&logoColor=61DAFB"> <img src="https://img.shields.io/badge/-339933?style=flat-square&logo=nodedotjs&logoColor=white"> <img src="https://img.shields.io/badge/-764ABC?style=flat-square&logo=redux&logoColor=white">
- **Language**: HTML5, CSS3, JavaScript
- **Framework/Library**: React, Redux Toolkit, Node.js
- **Network**: Axios, WebSocket (STOMP/SockJS)
- **UI/UX**: Chart.js, React Calendar, face-api.js

### **Data & AI** &nbsp; <img src="https://img.shields.io/badge/-003545?style=flat-square&logo=mariadb&logoColor=white"> <img src="https://img.shields.io/badge/-DC382D?style=flat-square&logo=redis&logoColor=white"> <img src="https://img.shields.io/badge/-000000?style=flat-square&logo=ollama&logoColor=white"> <img src="https://img.shields.io/badge/-412991?style=flat-square&logo=openai&logoColor=white">
- **DataBase**: MariaDB, Redis
- **AI/LLM**: OpenAI API, LangChain, Ollama
- **Data Analysis**: Pandas, NumPy, Matplotlib, OpenCV, PyMySQL

### **Tools** &nbsp; <img src="https://img.shields.io/badge/-F05032?style=flat-square&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white"> <img src="https://img.shields.io/badge/-F24E1E?style=flat-square&logo=figma&logoColor=white">
- **IDE**: IntelliJ, Cursor, VSCode, WebStorm
- **Collaboration**: Git, GitHub, Figma, Postman, Swagger
- **Database Tools**: MySQL Workbench


## 4. 🗂️ ERD (Entity Relationship Diagram)

> 프로젝트 데이터베이스 설계도입니다.
> <img width="3181" height="2728" alt="KakaoTalk_20260114_113027856" src="https://github.com/user-attachments/assets/908ec8cc-2a42-482d-aba8-210656ac0541" />

## 5. 🏗️ 프로젝트 구조 (Use Case Diagram)

> 사용자와 관리자의 주요 행동 흐름을 정의한 유스케이스 다이어그램입니다.
> ![KakaoTalk_20260113_150056077](https://github.com/user-attachments/assets/2c897d6e-8b7e-430f-be97-b8a31b27f617)



## 6. 🏛️ 시스템 아키텍처 (System Architecture)

> **AI 기반 업무 처리 및 실시간 통신 흐름**



## 7. 📺 기능 소개 및 시연

### 📂 팀 프로젝트 포트폴리오 (PDF)

> 프로젝트의 상세 기획 및 구현 과정이 담긴 PDF입니다.

- [📄 포트폴리오 다운로드](./모노크롬*미니멀리스트*포트폴리오\_프레젠테이션.pdf) _(파일 경로를 맞춰주세요)_

### 🎥 시연 영상

> 주요 기능 시연 영상입니다.

- [▶️ Youtube Link](https://youtube.com...) _(링크를 추가해주세요)_

## 8. ✨ 핵심 구현 기능 (Implemented Features)

### 1️⃣ AI 회의록 분석 및 Todo 자동 생성

- 회의록 파일을 업로드하면 AI가 내용을 분석하여 중요 과제를 추출합니다.
- 추출된 과제는 Todo List와 캘린더에 자동으로 등록됩니다.

### 2️⃣ 영수증 OCR 및 경비 처리

- 영수증 사진을 업로드하면 OCR 기술(Python AI 서버)이 상호명, 금액, 날짜 등을 자동 추출합니다.
- 수기 입력 없이 간편하게 경비 지출 내역을 등록할 수 있습니다.

### 3️⃣ AI 지출 결재 추천 시스템

- 등록된 지출 내역과 영수증 정보를 AI가 사내 규정과 비교 분석합니다.
- 관리자에게 **[승인 / 반려 / 보류]** 여부를 추천하고, 위험 요소를 분석하여 리포트를 제공합니다.

### 4️⃣ 실시간 채팅 및 AI 검색 (RPA)

- WebSocket(STOMP) 기반의 개인/부서별 실시간 채팅을 지원합니다.
- **AI 전역 검색**: 채팅방의 대화 맥락을 AI가 파악하여, 과거 대화 내용이나 공유된 파일을 자연어 질문으로 찾을 수 있습니다.

### 5️⃣ 기타 편의 기능

- **얼굴 인식 로그인**: face-api.js를 활용한 생체 인식 로그인
- **대시보드**: 개인별 업무 현황, 결재 대기 건수 등을 한눈에 파악하는 반응형 대시보드

## 9. 🚀 배포 (Deployment)

- **배포 기간**: 2026.01.13 ~ 2026.01.16
- _(AWS, Vercel 등 배포 환경에 대한 설명이나 링크를 이곳에 추가하세요)_

---

[cite_start]_Created by Team 1 (SmartSpend)_ [cite: 4, 8]
