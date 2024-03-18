## 🙌 올림 프로젝트 CRM
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219293363501535363/2023-12-26_143330.png?ex=660ac66f&is=65f8516f&hm=99f744e1e9d97969c392296d1fa1eca9ba2ea903d8df684fd901620e6dfcc191&" alt="drawing" width="400"/>

#### 올림 프로젝트는 개발 중단된 프로젝트입니다. 아래 웹 사이트를 통해 테스트할 수 있습니다.
#### [Github 조직](https://github.com/Olim-org) 
#### [Website](https://olim-crm-front.vercel.app/introduction)


## 🏢 TEAM
- ### Backend 
  - 허재우 (CSE, UNIST)
    - [Github](https://github.com/wodn1478)
    - Email: wodn14789@naver.com
- ### Frontend 
  - 황찬휘 (CSE, UNIST)
    - [Github](https://github.com/chan-hwi)
    - Email: gazebo5@naver.com


## ❓ 무인 헬스장 맞춤 CRM

## 🛠 기술 스택 - Backend
  - Java 21
  - Spring Boot (3.2.2)
  - Spring Web
  - Spring Data JPA
  - Spring Cloud
  
  - Jwt
  - Spring Security
  
  - Mysql
  - Redis

  - Open API Swagger
## 🔅 프로젝트 구조
### Backend
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219311405996441691/image.png?ex=660ad73c&is=65f8623c&hm=7f8d08e0e9eb2ad97379e8c481608ee48b9f9f7c35843db2aa82bfe9df8230e4&" alt="drawing" width="600"/>

#### [OlimGateway](https://github.com/Olim-org/OlimGateway-source.git)
  - **Gateway**: 백엔드와 프론트의 통신문
  - **기능**: API 라우팅, 유저 인증 및 권한 확인, 로드밸런싱
#### [OlimAuth-service](https://github.com/Olim-org/OlimAuth-source.git)
  - **기능**:
    - 유저의 회원가입, 로그인 등 인증 및 인가를 관리합니다.
    - JWT (access token + refresh token) 발급 및 Redis를 통해 refresh를 저장합니다.
    - 저장된 리프레시 토큰은 1번 사용되면 다시 재발급 + 재저장 됩니다.
    - 이미지 업로드를 위한 S3 업로드 서비스가 포함되어 있습니다.
    - 유저 프로필 관리 및 이메일 서비스도 함께 포함되어 있습니다.
    - Swagger API [링크](https://apis.olim.pyre.live/auth-service/swagger-ui/index.html)
#### [OlimCustomer-service](https://github.com/Olim-org/OlimCustomer-service.git)
  - **기능**:
    - CRM 회원과 관련된 기능을 제공합니다.
    - Swagger API [링크](https://apis.olim.pyre.live/customer-service/swagger-ui/index.html)
#### [OlimReserve-service](https://github.com/Olim-org/OlimReserve-service.git)
  - **기능**:
    - 헬스장 이용권 관련 기능을 제공합니다.
    - Swagger API [링크](https://apis.olim.pyre.live/reserve-service/swagger-ui/index.html)

