# Orca

# 🌟 StarVive_BE – Backend

> 스타벅스 앱 기반 이커머스 플랫폼 백엔드 리빌딩 프로젝트  
> Spring Boot 기반의 RESTful API 서버입니다.

---

## 🔗 프로젝트 링크

- **Backend Repository**: [https://github.com/1-StarVive/StarVive_BE](https://github.com/1-StarVive/StarVive_BE)

---

## 📌 프로젝트 개요

StarVive는 스파로스 아카데미에서 진행된 팀 프로젝트로,  
**스타벅스 앱 온라인 스토어**를 리빌딩하여 **모바일 중심의 이커머스 서비스**를 구현하였습니다.

> 주요 기능: 회원가입, 로그인(JWT), 상품 조회, 카테고리별 조회, 장바구니, 추천 섹션 , 찜하기 등

---

## 🚀 기술 스택

### 🔧 Backend
- Spring Boot 3.3.1
- Java 17
- Gradle (Groovy)
- Spring Data JPA
- Spring Security + JWT
- Redis (캐시, 세션 처리)
- Swagger (Springdoc OpenAPI)

### 🛠 Infra
- MySQL 8.0+
- Redis 6.2+
- AWS EC2, S3
- Jenkins + Docker
- Nginx (HTTPS 리버스 프록시)

---

## 🧰 실행 방법

### 1. 레포지토리 클론
```bash
git clone https://github.com/1-StarVive/StarVive_BE.git
cd StarVive_BE
2. Gradle 빌드
bash
복사
편집
./gradlew clean build
3. application.yml 설정
application-example.yml 참고하여 src/main/resources/application.yml 생성

yaml
복사
편집
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/starvive_database
    username: your_user
    password: your_password
  redis:
    host: localhost
    port: 6379

jwt:
  secret: your_jwt_secret
4. 서버 실행
bash
복사
편집
./gradlew bootRun
5. Swagger UI 확인
bash
복사
편집
http://localhost:8080/swagger-ui/index.html

주요 기능

회원가입 / 로그인 / 로그아웃 (JWT + 이메일 인증)

상품 목록 / 상세 / 옵션 / 썸네일 이미지

장바구니 CRUD

주문 생성 / 조회 / 상태 변경

찜하기 기능 (Redis + Spring Batch 기반 랭킹)

추천 섹션 및 상품 등록/조회

배너 이미지 업로드 (S3 연동)

Swagger 기반 API 문서화

📦 CI/CD
GitHub Actions + Jenkins 자동화 빌드

Docker 이미지 빌드 및 AWS EC2 배포

HTTPS: Nginx 리버스 프록시 + 인증서 설정

## 🛠️ 기술 스택

### Back-End

![Java](https://img.shields.io/badge/Java-17-007396?style=flat-square&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.1.x-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-7.x-02303A?style=flat-square&logo=gradle&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-Secured-6DB33F?style=flat-square&logo=spring-security&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-Authorization-000000?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-8.0+-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-6.2+-DC382D?style=flat-square&logo=redis&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-UI-85EA2D?style=flat-square&logo=swagger&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-Container-2496ED?style=flat-square&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-CI/CD-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Amazon EC2](https://img.shields.io/badge/AWS%20EC2-Cloud-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![Amazon S3](https://img.shields.io/badge/AWS%20S3-Storage-569A31?style=flat-square&logo=amazon-aws&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-ReverseProxy-009639?style=flat-square&logo=nginx&logoColor=white)
