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
- 무인 헬스장에 맞게 점주들의 헬스장 관리를 도와주는 웹 사이트입니다.
- 회원, 강사 관리, 이용권 관리, 출석 관리, 센터 관리 및 통계를 제공합니다.
- CRM 사이트에서 회원가입 후 자신만의 센터를 만들어보세요.
- 센터는 여러 개 등록할 수 있습니다.

[센터 기능 이미지로 구경하기](#image)

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


## CRM 이미지 (#image)

### - CRM 메인 화면

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219464238066569320/image.png?ex=660b6592&is=65f8f092&hm=36cfba1d0b6e428c12a538f323b4f1fcc75fa8fe6e0da149db0a11e450fd8e20&" alt="drawing" width="800"/>

### - 센터 간편 등록

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219464444900278353/image.png?ex=660b65c4&is=65f8f0c4&hm=afb257da7dd7d2caafdeb9ad4a3fd58eacdf815beef19dd6302e6a7a9ce08fcc&" alt="drawing" width="800"/>

### - 센터 메인 화면

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219466096407613491/image.png?ex=660b674d&is=65f8f24d&hm=9faff97ccb14c4e62155d983d4d4d55d0159f1eb12eecfdc29c3e7665d1028b9&" alt="drawing" width="800"/>

### - 회원 추가 화면

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219466354596380672/image.png?ex=660b678b&is=65f8f28b&hm=0ddbc4c7668360f627349052c6fbef373b79bb71a6672bb15290ed3609ba90b8&" alt="drawing" width="800"/>

### - 회원 상세정보 관리

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219466564529815592/image.png?ex=660b67bd&is=65f8f2bd&hm=e6c57a09c106fa51e5bc131e1262e796a4782b5455c925f796dbb517cd9b9231&" alt="drawing" width="800"/>
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219466679046635620/image.png?ex=660b67d8&is=65f8f2d8&hm=227ef74a399aaa5da72fe5c1719c142bb612b4d4c8f0ed2c77baa5582e621328&" alt="drawing" width="800"/>

### - 고객 이용권 추가 화면

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219468380830961774/image.png?ex=660b696e&is=65f8f46e&hm=86b738d5e24567133b0d356bfbc61bb4b30fe271d2abbd3c47a38233bda3afbb&" alt="drawing" width="800"/>
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219468606295773204/image.png?ex=660b69a4&is=65f8f4a4&hm=ecb0f05370e02f6eb94745b11e2d0360b6310e46386f337d6c99048f56cd84cb&" alt="drawing" width="800"/>

### - 출석 체크 기능 (이용권 필요)

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219467659998007336/image.png?ex=660b68c2&is=65f8f3c2&hm=e9685fa7ffc832286ba632a30add0c9c87c3bb734a898e5be7adccff6d9306c3&" alt="drawing" width="800"/>
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219467677236727808/image.png?ex=660b68c6&is=65f8f3c6&hm=0001f7f348dc76267d10b66f31f9cc6f55b06c643539b315dbba26cd7cf15153&" alt="drawing" width="800"/>
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219469872577122314/image.png?ex=660b6ad2&is=65f8f5d2&hm=fc495c2e343848f2c4fdc7f7ea89c1ffeda0101407074f4adae024437f5cdce0&" alt="drawing" width="800"/>

### - 센터 관리 기능

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219470178908377138/image.png?ex=660b6b1b&is=65f8f61b&hm=99644d07278963446dcbf57849428912ccfa5de03334eccee9e04f943ca79e55&" alt="drawing" width="800"/>

### - 강사 관리 기능

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219470309510610974/image.png?ex=660b6b3a&is=65f8f63a&hm=b4fe75d27864cb7fd94d5fe49b445be56e097dacc69f65fda5727e3b0942280b&" alt="drawing" width="800"/>

### - 센터 대시보드 (통계)

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219471011590701076/image.png?ex=660b6be1&is=65f8f6e1&hm=cbc0b9ae96565204a63f5a03a4da8a474d81a43185e1d633c6a5d7534fd168c9&" alt="drawing" width="800"/>
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219471153970806836/image.png?ex=660b6c03&is=65f8f703&hm=9d7f39d81e11aa2745ba4556447eb84bef135178901a3de45adefbb50908eba4&" alt="drawing" width="800"/>

### - 이용권 관리 기능

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219471454786158754/image.png?ex=660b6c4b&is=65f8f74b&hm=3321cf54dd387059bc5ade4e3a6a84bc201a09fcfe051262496e60058e0d1ae2&" alt="drawing" width="800"/>
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219471859117199400/image.png?ex=660b6cab&is=65f8f7ab&hm=a582f39e8d6befa60d7e6a85ab36278048e392f3cb96b9f5c41815749c756a33&" alt="drawing" width="800"/>
<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219471843136770169/image.png?ex=660b6ca8&is=65f8f7a8&hm=817601411addd7c53b9d7accf8670ea79c527203526eac8a96576ae1fab2edd1&" alt="drawing" width="800"/>

### - 이용권 별 출석 현황

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219472081448861726/image.png?ex=660b6ce0&is=65f8f7e0&hm=80403f15e3ae722605871e4fc6afa177d628f52aab29089dad0bf4781d0aa000&" alt="drawing" width="800"/>

### - 이용권 사용 통계

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219472235266314371/image.png?ex=660b6d05&is=65f8f805&hm=02eba9f5285a5a9f0cfe033cb6dcbf2cd88a9d1417766b5e5e7beb7079b48222&" alt="drawing" width="800"/>

### - 이용권 구매 현황

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219472537751126057/image.png?ex=660b6d4d&is=65f8f84d&hm=4073238af925cd5ad3a112fe9f99086f57ccba2df4c10646040f8ddd86215870&" alt="drawing" width="800"/>

### - 간편한 타 지점 전환

<img src="https://cdn.discordapp.com/attachments/393025698907947009/1219473216561479760/image.png?ex=660b6def&is=65f8f8ef&hm=6da00a8e389d6fbbb738e9bee98461766c72773dd5f8dc580b821c00e31e5541&" alt="drawing" width="800"/>
