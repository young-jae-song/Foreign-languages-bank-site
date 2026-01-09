# 외국어 문제 풀이 웹 서비스 (Capstone Design)

---

## 1. 프로젝트 개요

본 프로젝트는 일반 사용자를 위한 외국어 문제 풀이 서비스와  
관리자를 위한 문제 및 사용자 관리 기능을 제공하는 웹 기반 서비스입니다.

- Node.js 서버 기반 실행
- Bootstrap(SB Admin 2) 관리자 템플릿 적용
- LocalStorage 기반 문제 데이터 관리
- 관리자 / 일반 사용자 권한 분리

---

## 2. 사용 기술

### Backend
- Node.js

### Frontend
- HTML
- CSS
- JavaScript
- Bootstrap (SB Admin 2)

### Data
- Browser LocalStorage

---

## 3. 실행 환경

- OS: Windows / macOS
- Node.js: 18.x 이상
- Browser: Chrome 권장

---

### 4. 프로젝트 구조
```bash
startbootstrap-sb-admin-2-gh-pages/
 ├─ server.js              # Node.js 서버 실행 파일
 ├─ package.json           # 프로젝트 의존성 정보
 ├─ login.html             # 로그인 페이지
 ├─ index.html             # 일반 사용자 문제 풀이 페이지
 ├─ charts.html            # 관리자 문제 관리 페이지
 ├─ js/                    # JavaScript 파일
 ├─ css/                   # 스타일 파일
 └─ vendor/

```
---

## 5. 프로젝트 실행 방법

### 5-1. 프로젝트 경로 이동

```bash
cd 다운로드/캡스톤디자인/startbootstrap-sb-admin-2-gh-pages
```

### 5-2. 의존성 설치
npm install

### 5-3. 서버 실행
node server.js

### 5-4. 접속 주소
http://localhost:3000

---

### 6. 주요 기능 요약
- 일반 사용자 기능

- 로그인 후 즉시 문제 풀이 가능

- 언어 선택 가능 (영어 / 일본어 / 중국어)

- 언어별 100문제 제공 (총 300문제)

- 객관식 4지선다 문제 구성

- 정답 선택 시 즉시 결과 확인

- 관리자 기능

- 문제 추가 / 수정 / 삭제

- 문제 과목 관리

- 문제 난이도 관리

- 사용자 정보 확인

- 사이트 통계 확인

---

## 7. 로그인 계정 정보
- 일반 사용자

  ID: user01

  PW: pass1234

- 관리자

  ID: admin

  PW: admin1234

## 8. 일반 사용자 화면

- 로그인 후 문제 풀이 페이지로 이동

- 문제는 자동으로 로드됨

- 관리자 페이지 접속 여부와 무관하게 문제 풀이 가능

## 9. 관리자 주요 역할

- 문제 추가 / 수정 / 삭제

- 문제 과목 관리

- 문제 난이도 관리

- 사용자 정보 확인

- 사이트 통계 확인

---

### 10. 문제 데이터 관리 구조

- 데이터 저장 위치: Browser LocalStorage

- 사용 Key: questions

- 관리자 페이지 최초 접속 시 기본 문제 자동 생성

- 생성된 문제는 일반 사용자 페이지에 즉시 반영

- 기본 문제 구성

- 영어 100문제

- 일본어 100문제

- 중국어 100문제

---



## 11. 관리자 페이지 사이트맵
```bash
[관리자 페이지 구조]
관리자 페이지
│
├─ Dashboard
│   └─ 서비스 현황 요약
│
├─ User Management
│   ├─ 일반 사용자 목록 조회
│   ├─ 사용자 계정 관리
│
├─ Question Management
│   ├─ 문제 등록
│   ├─ 문제 수정
│   ├─ 문제 삭제
│   └─ 언어별 문제 관리
│
├─ Data Charts
│   └─ 문제 데이터 시각화
│
└─ Settings
    └─ 서비스 설정

```

---

### 12. 프로젝트 특징

- 별도 데이터베이스 없이 실행 가능

- 관리자 페이지를 통한 실시간 문제 관리

- 권한별 화면 분리

- 실행 및 배포가 간단한 구조

---

### 13. 향후 개선 사항

데이터베이스 연동 (MySQL / MongoDB)

로그인 보안 강화

문제 풀이 이력 저장

통계 시각화 고도화
