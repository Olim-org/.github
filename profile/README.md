## 🙌 올림 프로젝트 CRM

<img src="https://github.com/user-attachments/assets/52496cb9-12d3-4f4d-9fa3-8f2b692df7b4" alt="drawing" width="400"/>

#### 올림 프로젝트는 개발 중단된 프로젝트입니다. ~~아래 웹 사이트를 통해 테스트할 수 있습니다.~~
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
- 무인 헬스장에 맞게 점주들의 헬스장 관리를 도와주는 웹 사이트입니다.
- 회원, 강사 관리, 이용권 관리, 출석 관리, 센터 관리 및 통계를 제공합니다.
- CRM 사이트에서 회원가입 후 자신만의 센터를 만들어보세요.
- 센터는 여러 개 등록할 수 있습니다.

[센터 기능 이미지로 구경하기](#crm-이미지)

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

<img src="https://github.com/user-attachments/assets/b99cfb09-42ce-4491-9b77-b1b3706ed2d4" alt="drawing" width="600"/>

#### [OlimGateway](https://github.com/Olim-org/OlimGateway-source.git)
  - **Gateway**: 백엔드와 프론트의 통신문
  - **기능**: API 라우팅, 유저 인가, 로드밸런싱
#### [OlimAuth-service](https://github.com/Olim-org/OlimAuth-source.git)
  - **기능**:
    - 유저의 회원가입, 로그인 등 인증 및 인가를 관리합니다.
    - JWT (access token + refresh token) 발급 및 Redis를 통해 refresh를 저장합니다.
    - 저장된 리프레시 토큰은 1번 사용되면 다시 재발급 + 재저장 됩니다.
    - 이미지 업로드를 위한 S3 업로드 서비스가 포함되어 있습니다.
    - 유저 프로필 관리 및 이메일 서비스도 함께 포함되어 있습니다.
    - ~~Swagger API [링크](https://apis.olim.pyre.live/auth-service/swagger-ui/index.html)~~
#### [OlimCustomer-service](https://github.com/Olim-org/OlimCustomer-service.git)
  - **기능**:
    - CRM 회원과 관련된 기능을 제공합니다.
    - ~~Swagger API [링크](https://apis.olim.pyre.live/customer-service/swagger-ui/index.html)~~
#### [OlimReserve-service](https://github.com/Olim-org/OlimReserve-service.git)
  - **기능**:
    - 헬스장 이용권 관련 기능을 제공합니다.
    - ~~Swagger API [링크](https://apis.olim.pyre.live/reserve-service/swagger-ui/index.html)~~

# CRM 이미지

### - CRM 메인 화면

<img src="https://github.com/user-attachments/assets/ca78f3dd-bdf4-4092-9dd8-910ae196483c" alt="drawing" width="900"/>

### - 센터 간편 등록

<img src="https://github.com/user-attachments/assets/d1c9c7db-f44a-4091-86f8-24f307f733ad" alt="drawing" width="900"/>

### - 센터 메인 화면

<img src="https://github.com/user-attachments/assets/15c11bb4-6c4e-4d20-8330-f1ac5e6eab6c" alt="drawing" width="900"/>

### - 회원 추가 화면

<img src="https://github.com/user-attachments/assets/79ffee82-b23a-4f08-8e9d-33eabad01e7b" alt="drawing" width="900"/>

### - 회원 상세정보 관리

<img src="https://github.com/user-attachments/assets/a00955c6-6437-4176-b49f-21be7cc08394" alt="drawing" width="900"/>
<img src="https://github.com/user-attachments/assets/89d7b108-53e5-4806-9faf-a2f074c1ea83" alt="drawing" width="900"/>

### - 고객 이용권 추가 화면

<img src="https://github.com/user-attachments/assets/a6f2bb92-4319-49b0-beb2-6ce3538c5f91" alt="drawing" width="900"/>
<img src="https://github.com/user-attachments/assets/a4839340-903f-435a-b0bf-f9fdae4f2df9" alt="drawing" width="900"/>

### - 출석 체크 기능 (이용권 필요)

<img src="https://github.com/user-attachments/assets/32a6954b-a64d-47ac-8ea2-de8be9efad1a" alt="drawing" width="900"/>
<img src="https://github.com/user-attachments/assets/135f5b83-3b59-40f9-bbae-2d532844b672" alt="drawing" width="900"/>
<img src="https://github.com/user-attachments/assets/1dc9c10f-9bbd-4904-8e6d-820fa84adb18" alt="drawing" width="900"/>

### - 센터 관리 기능

<img src="https://github.com/user-attachments/assets/40299eb2-23a5-4ef7-bc6c-dcdc8e8d40af" alt="drawing" width="900"/>

### - 강사 관리 기능

<img src="https://github.com/user-attachments/assets/4a22e8c2-fa97-4fec-8e1e-9a462a8ceeae" alt="drawing" width="900"/>

### - 센터 대시보드 (통계)

<img src="https://github.com/user-attachments/assets/ef5c03de-c622-4f71-bfbd-86dabd11237e" alt="drawing" width="900"/>
<img src="https://github.com/user-attachments/assets/04650b94-4aee-45e2-9623-fc80cd854d37" alt="drawing" width="900"/>

### - 이용권 관리 기능

<img src="https://github.com/user-attachments/assets/503fa1c3-881e-45bb-b113-0e2ab1a29c19" alt="drawing" width="900"/>
<img src="https://github.com/user-attachments/assets/9795e170-7988-4b29-bd18-972023cd7f18" alt="drawing" width="900"/>
<img src="https://github.com/user-attachments/assets/ed707cb8-019e-4038-9f69-c02e4d37d879" alt="drawing" width="900"/>

### - 이용권 별 출석 현황

<img src="https://github.com/user-attachments/assets/242fa07f-64f3-4c66-aa9c-a07f463525b0" alt="drawing" width="900"/>

### - 이용권 사용 통계

<img src="https://github.com/user-attachments/assets/b55b32a1-d4d2-4750-9402-8e677926c30b" alt="drawing" width="900"/>

### - 이용권 구매 현황

<img src="https://github.com/user-attachments/assets/20cd84f1-6c2b-4802-aea6-e4b98d4c4927" alt="drawing" width="800"/>

### - 간편한 타 지점 전환

<img src="https://github.com/user-attachments/assets/8ebdcb55-541a-4ab8-9fc2-20718306ff64" alt="drawing" width="800"/>
