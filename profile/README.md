# Link-Buddy (링크 버디)
<p align="center">
  <img width="30%" alt="logo_main" src="https://github.com/user-attachments/assets/93591328-14c9-4344-885c-8a4b1a71782c">
</p>

## 📚 Repository
* Backend: [Link-Buddy/back](https://github.com/Link-Buddy/back)
* Frontend: [Link-Buddy/front](https://github.com/Link-Buddy/front)

## 📖 목차
1. [프로젝트 소개](#프로젝트-소개)
   - [주요 기능](#주요-기능)
   - [프로젝트 목적](#프로젝트-목적)
   - [개발 기간](#개발-기간)
   - [팀원 구성](#팀원-구성)
2. [스토리보드](#스토리보드)
3. [Frontend](#frontend)
   - [사용기술](#frontend-사용기술)
   - [폴더구조](#frontend-폴더구조)
   - [주요기능](#frontend-주요기능)
4. [Backend](#backend)
   - [사용기술](#backend-사용기술)
   - [ERD](#erd)
   - [폴더구조](#backend-폴더구조)
   - [주요기능](#backend-주요기능)
   - [이슈사항](#이슈사항)

## 프로젝트 소개
링크 공유 플랫폼

이 프로젝트는 Spring Boot와 React를 사용하여 개발했습니다.
내 링크를 관리하고 친구를 초대해 링크를 공유할 수 있는 링크 공유 플랫폼 사이트입니다.
(참고: [JOOSUM](https://letspl.me/booth/joosum/JOOSUM))

### 주요 기능
- 친구와 링크를 공유
- 내 링크 관리

### 프로젝트 목적
- Spring Boot, React 기반 개발 경험 축적

### 개발 기간
- 전체 개발 기간 : 2024.01.07 ~ 2025.01
- 기획 (주제 선정, 디자인, 스토리보드 및 ERD 구성) : 2024.01.07 ~ 2024.02.04
- Backend 작업 : 2024.02.11 ~ 2024.06.16
- Frontend 작업 : 2024.06.22 ~ 2025.01.11

### 팀원 구성
- https://github.com/yl9517
- https://github.com/yjink12

## 스토리보드
<div style="display: flex; gap: 40px; justify-content: center;">
    <img alt="storyboard1" src="https://github.com/user-attachments/assets/fbea1616-235b-4e4e-8283-f2b891fa0a7b" style="width: 40%;">
    <img alt="storyboard2" src="https://github.com/user-attachments/assets/69e50089-db3f-4344-bc67-1b7d2455a36c" style="width: 45%;">
</div>

## Frontend

### Frontend 사용기술
- Framework/Language: React(v18.2.0), Typescript
- UI: Ant Design (Antd), Tailwind CSS

### Frontend 폴더구조
```bash
/src
  ├── /assets
  │   └── /images  #이미지, 폰트, 아이콘 등의 정적 파일
  ├── /components  # 재사용 가능한 UI 컴포넌트
  │   └── /layout 
  │   └── /button
  │   └── /card
  ├── /hooks      # 커스텀 훅
  ├── /pages      # 페이지별 컴포넌트
  ├── /utils      # 유틸리티 함수
  ├── /styles     # 스타일링 파일
  ├── /api        # API 호출 관련 로직
  ├── /routes     # 라우팅 설정
  ├── /types      # 타입 정의
  ├── /store      # React Context API
  ├── /lib        # 프로젝트 공통 로직
  └── App.js
```

### Frontend 주요기능
1. 홈
   - 즐겨찾기
   - 오늘의 링크 추가
     - 링크 추가일마다 링크 추가 도장 표시
    <p align="center">
      <img width="40%" alt="main" src="https://github.com/user-attachments/assets/1a097da6-f159-4c40-baea-fe95de663b9b">
    </p>
  - 검색
    <p align="center">
      <img width="40%" alt="search" src="https://github.com/user-attachments/assets/a2f19045-495e-4cc3-967c-12671d614d23">
    </p>

2. 로그인 & 회원가입
   - 회원가입 → 로그인
     <p align="center">
      <img width="40%" alt="login" src="https://github.com/user-attachments/assets/fd6d6238-c31f-41e6-819b-4befb01d0356">
    </p>
   - 간편로그인 (구글, 네이버)

3. 버디링크
   - 친구 초대
     <p align="center">
      <img width="40%" alt="invite" src="https://github.com/user-attachments/assets/d6429016-db8b-431a-bb25-de479c6640c8">
    </p>
   - 버디 추가
   - 버디 설정
     <div style="display: flex; gap: 40px; justify-content: center;">
      <img alt="buddy1" src="https://github.com/user-attachments/assets/d4aef135-b6a8-4033-8a83-fdcc8cfbb01b" style="width: 40%;">
      <img alt="buddy2" src="https://github.com/user-attachments/assets/aa4986f4-48f4-4af4-bf6b-4f10f8303fef" style="width: 45%;">
    </div>

4. 내 링크
   - 링크 추가, 수정, 삭제
     <p align="center">
      <img width="40%" alt="link_add" src="https://github.com/user-attachments/assets/894ba6fe-4aa7-4f7c-a870-509030d21f60)">
    </p>
   - 링크 즐겨찾기
   - 링크 폴더 이동 가능
     <p align="center">
      <img width="40%" alt="link_move" src="https://github.com/user-attachments/assets/695a5b7b-f984-4544-a7f0-495ee7dd433c">
    </p>

## Backend

### Backend 사용기술
- Framework/Language: Spring Boot, Java(v17.0.9)
- DB관련: MariaDB, JPA, QueryDSL
- Tool: DBeaver

### ERD
<p align="center">
      <img width="80%" alt="erd" src="https://github.com/user-attachments/assets/b57262f8-05d0-4458-894e-3492ceb778a3">
    </p>

### Backend 폴더구조
```jsx
src/
└── main/
    └── java/
        └── com/
            └── linkbuddy/
                ├── config/                  # 애플리케이션 설정 파일들
                ├── common/                  # 전역적으로 사용되는 공통 클래스들
                ├── domain/                  # 도메인별 폴더
                    ├── buddy/              # 'Buddy' 도메인
                        ├── dto/            # Data Transfer Objects
                        ├── entity/         # JPA 엔티티 클래스
                        ├── repository/     # Spring Data JPA 리포지토리
                        ├── service/        # 비즈니스 로직
                        └── controller/     # HTTP 요청 처리
                    ├── anotherdomain/     # 다른 도메인
                        ├── ...
                ├── Application.java        # 애플리케이션 메인 클래스
└── resources/
```

### Backend 주요기능
- 간편 로그인 (구글, 네이버)
  - Spring Security + JWT + Oauth2
- 로그인 & 회원가입

### 이슈사항
- [[Spring boot] Spring Security 3.x.x + JWT ](https://www.notion.so/Spring-boot-Spring-Security-3-x-x-JWT-5485f360e1e24726a018125e72a8b33e?pvs=21)
- [[Spring boot] OncePerRequestFilter와 Filter의 차이](https://www.notion.so/Spring-boot-OncePerRequestFilter-Filter-2664db6691cb46e8803a30c91988229d?pvs=21)
- [[Spring boot] Ouath2](https://www.notion.so/Spring-boot-Ouath2-3ded56be98494a9b84aa725c1ee5a13f?pvs=21)
- [[241102] Link Preview](https://www.notion.so/241102-Link-Preview-efe8bc029fb74ae6a3849333f47be8a7?pvs=21)
- [[241019] SQL문 조건 위치에 따른 문제 해결](https://www.notion.so/241019-SQL-1240e2a0ccba8016a55bd0f64ed7a793?pvs=21)
