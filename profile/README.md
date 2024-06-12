# ☕ NFCOFFEE 

![1st](https://github.com/NFCoffee/.github/blob/main/profile/Images/1st.png)

<br>

## 프로젝트 소개

- NFCOFFEE는 기존 중앙집중식 서버 시스템의 한계를 해결하기 위한 블록체인 기반 모바일 오더 시스템입니다.
- NFT 발급을 활용하여 조직 내 신원 확인 기능을 제공합니다.
- 스마트 컨트랙트를 통해 안전하고 투명한 거래를 보장합니다.

<br>

## 팀원 구성

<div align="center">

| **이민규** | **이지인** | **박정진** | **장철희** | **조성열** |
| :------: |  :------: | :------: | :------: | :------: |
| [<img src="https://avatars.githubusercontent.com/u/76238096?v=4" height=150 width=150> <br/> @2mingyu](https://github.com/2mingyu) | [<img src="https://avatars.githubusercontent.com/u/80019560?v=4" height=150 width=150> <br/> @20massalia](https://github.com/20massalia) | [<img src="https://avatars.githubusercontent.com/u/109943960?v=4" height=150 width=150> <br/> @JeongjinP](https://github.com/JeongjinP) | [<img src="https://avatars.githubusercontent.com/jang-namu" height=150 width=150> <br/> @jang-namu](https://github.com/jang-namu) | [<img src="https://avatars.githubusercontent.com/u/145314175?v=4" height=150 width=150> <br/> @Choseongyul](https://github.com/Choseongyul) |

</div>

<br>

## 1. 개발 환경

- Front : React-Native(App), React(Block-explorer)
- Backend : springboot, node.js(web3)
- Blockchain: Solidity, go-ethereum
- 버전 및 이슈관리 : [Github](https://github.com/NFCoffee), Github Issues
- 협업 툴 : [Notion](https://nervous-clipper-604.notion.site/NFCoffee-c3d59d759eaf47a196f627cd1474d455?pvs=74)
- 디자인 : [Figma](https://www.figma.com/design/nJT0LMpzMuKb8IaddH8oBO/NFCoffee?node-id=1-2&t=MfJqnMSNEcUngKh4-1)
- 프로젝트 구조 : // todo

<br>

## 2. 채택한 개발 기술과 브랜치 전략

### Geth
- Go-ethereum
    - Ethereum의 smart contract를 구동할 수 있는 Go language로 개발된 클라이언트
    - Geth를 통한 블록의 트랜잭션을 검증하고 실행 가능

### Node.js
- web3.js
    - ABI 파일로 생성된 메타데이터로 Geth 네트워크 상 배포된 스마트-컨트랙트 호출(mintAndTransfer)
    - NFT 민팅 및 토큰 전송 API 제공

### Spring
- Java-mail-sender
    - 이메일 인증 서비스 구현, SMTP 사용
- Dockerize
    - jib 라이브러리 이용, Docker Image 형태로 프로젝트 빌드 및 배포


### React-Native

- React-Native
    - 컴포넌트화를 통해 추후 유지보수와 재사용성을 고려했습니다.
    - 유저 배너, 상단과 하단 배너 등 중복되어 사용되는 부분이 많아 컴포넌트화를 통해 리소스 절약이 가능했습니다.
- styled-component
    - props를 이용한 조건부 스타일링을 활용하여 상황에 알맞은 스타일을 적용시킬 수 있었습니다.
    - 빌드될 때 고유한 클래스 이름이 부여되어 네이밍 컨벤션을 정하는 비용을 절약할 수 있었습니다.
    - S dot naming을 통해 일반 컴포넌트와 스타일드 컴포넌트를 쉽게 구별하도록 했습니다.


### 브랜치 전략

- main 브랜치와 feature 보조 브랜치만으로 최대한 간결하게 유지하려 했습니다.
- main, Feat 브랜치로 나누어 개발을 하였습니다.
    - **main** 개발이 완료된 기능은 PR을 올려 main에 머지
    - **feat** 개발 기능 단위로 feature 브랜치 분리

<br>

## 4. 역할 분담

### 🍊이민규

- **Web3**
    - Geth 이용 Clique(PoA) 기반 Private Network 구성
    - Solidity 언어로 smart contracts 코드 작성 및 배포
- **기능**
    - nft 민팅 및 소유 확인
    - token 요청
    - token을 소모하여 음료 주문

<br>
    
### 💕박정진

- **논문**
    - 논문 작성 및 수정    

<br>

### 👻이지인

- **UI**
    - 페이지 : //todo
    - 공통 컴포넌트 : //todo
- **기능**
    - //todo

<br>

### 🍄조성열

- **UI**
    - 페이지 : //todo
    - 공통 컴포넌트 : //todo
- **기능**
    - //todo
    
<br>

### 🐬장철희

- **Backend**
    - node.js: nft minting - smart contarct 호출 API 제공
    - Spring: 이메일 기반 회원인증 및 가입, nft 민팅 API 호출
- **기능**
    - 회원가입, 스마트-컨트랙트 호출
    
<br>


## 5. 개발 기간 및 작업 관리

### 개발 기간

- 전체 개발 기간 : 2024-03-04 ~ 2024-05-31
- 기획 및 아키텍처 설계 : 2024-03-04 ~ 2024-03-18
- UI 구현 : 2024-03-18 ~ 2024-04-01
- 기능 구현 : 2024-04-01 ~ 2024-05-31

<br>

### 작업 관리

- GitHub Organzation에서 파트별 Projects, Issues를 사용하여 진행 상황을 공유했습니다.
- 매주 월요일 주간회의를 진행하며 작업 순서와 방향성에 대한 고민을 나누고 Figma와 노션에 회의 내용을 기록했습니다.

<br>

## 6. 개발 진행

- [Geth 이용 Clique(PoA) 기반 private network 구축](https://github.com/NFCoffee/.github/blob/main/profile/docs/Geth%20%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%AD%E1%86%BC%20Clique(PoA)%20%E1%84%80%E1%85%B5%E1%84%87%E1%85%A1%E1%86%AB%20private%20network%20%E1%84%80%E1%85%AE%E1%84%8E%E1%85%AE%E1%86%A8.pptx)

- [NFT, Token, Order 스마트 컨트랙트](https://github.com/NFCoffee/.github/blob/main/profile/docs/NFT%2C%20Token%2C%20Order%20%E1%84%89%E1%85%B3%E1%84%86%E1%85%A1%E1%84%90%E1%85%B3%20%E1%84%8F%E1%85%A5%E1%86%AB%E1%84%90%E1%85%B3%E1%84%85%E1%85%A2%E1%86%A8%E1%84%90%E1%85%B3.pptx)

| [Figma](https://www.figma.com/design/nJT0LMpzMuKb8IaddH8oBO/NFCoffee?node-id=1-2&t=MfJqnMSNEcUngKh4-1) | Swagger |
|----------|----------|
|![Figma](https://github.com/NFCoffee/.github/blob/main/profile/Images/figma.png)|![swagger](https://github.com/NFCoffee/.github/blob/main/profile/Images/swagger.png)|

- 프론트 이슈  
todo ..

<br>

## 7. NFCoffee 논문

[![Article](https://github.com/NFCoffee/.github/blob/main/profile/Images/Article.png?raw=true)](https://github.com/NFCoffee/.github/blob/main/profile/docs/NFCoffee_Article.pdf)

<br>


## 8. 페이지별 기능

### [초기화면]
- 어플리케이션 접속 초기화면입니다.
    - 로컬 스토리지에 암호화된 private key가 존재할 경우 : PIN 입력 후 Main 화면으로
    - 로컬 스토리지에 암호화된 private key가 존재하지 않을 경우 : 로그인 및 회원가입이 가능한 초기화면

| 초기화면 |
|----------|
|![초기화면](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_%EC%9D%B8%ED%8A%B8%EB%A1%9C.jpg)|

<br>

### [회원가입]
- 서비스 제공 조직의 데이터베이스와 연동하여, 사번(학번)으로 중복 가입을 방지하며, 이메일로 조직원 인증 후 가입합니다.

| 회원가입 | 메일 인증 |
|----------|----------|
|![회원가입](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_%ED%9A%8C%EC%9B%90%EA%B0%80%EC%9E%85.jpg)|![메일](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_%EB%A9%94%EC%9D%BC.gif)|

<br>

### [계정 생성]
- 로컬 스토리지에서 private key를 암호화/복호화 할 때 사용할 PIN 번호를 사용자에게 입력받습니다.
- web3.js 라이브러리를 이용해 블록체인 네트워크의 계정을 생성합니다.
- 계정의 주소를 백엔드로 보내면, NFT를 발급받게 됩니다.

| 계정 생성 |
|----------|
|![계정생성](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_%EA%B3%84%EC%A0%95.gif)|

<br>

### [Main]
- 상단 : NFT 보유 여부, 보유중인 PLZ 토큰 수량, PLZ 토큰 수령 버튼을 배치했습니다.
- 중단 : 퀵 오더에서 메뉴 이름을 선택하면, 해당 메뉴를 바로 주문할 수 있도록 Order 페이지로 이동합니다.
- 하단 : 최근 트랜잭션 기록을 간략히 표시합니다.

- 24시간에 한번 씩 토큰을 수령할 수 있습니다.
- 한번에 받을 수 있는 토큰의 수량은 조직에서 스마트 컨트랙트를 이용해 설정 가능합니다.

| Main | 토큰 수령 |
|----------|----------|
|![main](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_main.jpg)|![토큰수령](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_%ED%86%A0%ED%81%B0%EC%88%98%EB%A0%B9.gif)|

<br>

### [Order]
- 주문 가능한 메뉴들을 표시합니다.
- 품목을 선택한 후 주문하기 버튼을 클릭 시, 주문 내용이 블록체인 네트워크로 전송되며 토큰이 차감됩니다.

| Order | 주문 |
|----------|----------|
|![Order](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_order.jpg)|![주문](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_%EC%A3%BC%EB%AC%B8.gif)|

### [History]
- 사용자의 트랜잭션 기록이 전체 해시와 함께 표시됩니다.

| History |
|----------|
|![History](https://github.com/NFCoffee/.github/blob/main/profile/Images/%EC%8B%A4%ED%96%89%EC%98%81%EC%83%81_history.jpg)|

### [[Block Explorer](https://github.com/NFCoffee/block-explorer)]
- 자체 블록 탐색기를 개발하여 모든 트랜잭션 기록을 확인할 수 있게 했습니다.

| Block Explorer |
|-----------|
|![blockexplorer](https://github.com/NFCoffee/.github/blob/main/profile/Images/block%20explorer.png)|
