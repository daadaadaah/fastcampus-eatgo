# EatGo

[![Build Status](https://travis-ci.org/ahastudio/fastcampus-eatgo.svg?branch=master)](https://travis-ci.org/ahastudio/fastcampus-eatgo)

[“Fast Campus 올인원 패키지: Java 웹 개발 마스터” 실전 프로젝트.](https://www.fastcampus.co.kr/courses/200748/clips/)
- [패스트캠퍼스 온라인 스프링 부트 프로젝트 EatGo Reference](https://docs.google.com/document/d/e/2PACX-1vTStbhpexFdoJ4M7jHmaOge9V-iLuEXES22jZPdmZD-xgZr9p142xsreetWPhT94yh-E2RdGq0O964O/pub)

## Test all

```bash
SPRING_PROFILES_ACTIVE=test ./gradlew cleanTest test
```

## Build JAR

```bash
./gradlew bootJar
```

## Install dependencies for web

```bash
bash -c "cd eatgo-admin-web && npm install"
bash -c "cd eatgo-customer-web && npm install"
bash -c "cd eatgo-restaurant-web && npm install"
```

## Run with Docker

```bash
# Docker용 환경 설정 파일을 복사합니다.
# .env 파일은 필요에 따라 수정해서 사용하시면 됩니다.
cp .env.default .env

# 컨테이너를 모두 실행합니다.
docker-compose up
```

웹 프론트엔드 확인:

- Admin: <http://localhost:8082/>
- Customer: <http://localhost:8083/>
- Restaurant: <http://localhost:8084/>
