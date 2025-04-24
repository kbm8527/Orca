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


Swagger 기반 API 문서화

📦 CI/CD
GitHub Actions + Jenkins 자동화 빌드

Docker 이미지 빌드 및 AWS EC2 배포

HTTPS: Nginx 리버스 프록시 + 인증서 설정
```
---

## 🛠️ 기술 스택

### Back-End

<!-- Language & Framework -->
<img src="https://img.shields.io/badge/Java-17-007396?style=for-the-badge&logo=java&logoColor=white"/>
<img src="https://img.shields.io/badge/SpringBoot-3.1.x-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
<img src="https://img.shields.io/badge/Gradle-7.x-02303A?style=for-the-badge&logo=gradle&logoColor=white"/>

<!-- DB / Cache -->
<img src="https://img.shields.io/badge/MySQL-8.0+-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-6.2+-DC382D?style=for-the-badge&logo=redis&logoColor=white"/>

<!-- Security / Auth -->
<img src="https://img.shields.io/badge/Spring%20Security-Secured-6DB33F?style=for-the-badge&logo=spring-security&logoColor=white"/>
<img src="https://img.shields.io/badge/JWT-Authorization-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white"/>

<!-- Docs / Dev Tools -->
<img src="https://img.shields.io/badge/Swagger-API-85EA2D?style=for-the-badge&logo=swagger&logoColor=black"/>
<img src="https://img.shields.io/badge/Postman-TestTool-FF6C37?style=for-the-badge&logo=postman&logoColor=white"/>

<!-- DevOps -->
<img src="https://img.shields.io/badge/Docker-Container-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Jenkins-CI/CD-D24939?style=for-the-badge&logo=jenkins&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS%20EC2-Cloud-FF9900?style=for-the-badge&logo=amazon-ec2&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS%20S3-Storage-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white"/>
<img src="https://img.shields.io/badge/Nginx-ReverseProxy-009639?style=for-the-badge&logo=nginx&logoColor=white"/>

---
