# 🔐 Spring Security Board

> Spring Boot 기반의 간단한 게시판 웹 애플리케이션  
> 사용자 인증/인가 기능과 게시글 CRUD 기능을 포함하며, JPA 및 Spring Security 등 핵심 기술을 직접 적용해 구현했습니다.

---

## 🎯 개발 목적

- Spring Boot와 MVC 구조에 대한 이해를 높이기 위한 실습 프로젝트
- 로그인 인증과 게시글 CRUD 흐름을 직접 구현하며 백엔드 로직 학습
- Spring Data JPA와 Security 설정 경험 및 계층별 아키텍처 설계 연습

---

## 🛠 기술 스택

- **Java 17**
- **Spring Boot**
- **Spring Security**
- **Spring Data JPA**
- **JSP / Servlet**
- **H2 / MySQL**
- **Maven**

---

## 🔑 주요 기능

- 사용자 로그인 / 로그아웃
- 게시글 등록, 목록 조회, 상세 보기
- 게시글 수정 및 삭제
- DB 연동 및 게시글 로그 저장
- Spring Security 기반 인증 및 접근 권한 제어

---

## 🚀 실행 방법

1. DB 설정 확인  
   - `src/main/resources/application.yml`에서 DB 관련 설정을 환경에 맞게 수정

2. 프로젝트 실행
   ```bash
   ./mvnw spring-boot:run
   ```
3. 접속
   - 브라우저에서 http://localhost:8080 접속

## 📁 프로젝트 구조

```
src/
├── main/
│   ├── java/
│   │   └── edu.fisa.board/
│   │       ├── BoardApplication.java
│   │       ├── config/               # Security 설정
│   │       ├── controller/           # 로그인 & 게시판 컨트롤러
│   │       ├── entity/               # 게시글 Entity
│   │       ├── repository/           # JPA Repository
│   │       └── service/              # 비즈니스 로직
│   ├── resources/
│   │   └── application.yml           # DB 및 환경 설정
│   └── webapp/
│       └── WEB-INF/views/           # JSP 뷰 파일
├── test/
```

---

## 📌 참고 사항
최초 실행 시 기본적으로 H2 DB를 사용하며, application.yml을 수정해 MySQL 등으로 변경 가능합니다.

JSP 기반 구조이므로 Spring Boot Devtools 사용 시 자동 리로드 기능이 제한될 수 있습니다.

---

## ✨ 느낀 점
> Spring Security의 인증 구조와 세션 관리, MVC 아키텍처의 구성, 계층 분리 설계 등을 실무에 가깝게 체험할 수 있었습니다.
