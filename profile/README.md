# 🛍️ 중고 물품 경매 프로젝트 - 땅땅땅!

중고 물품을 경매 서비스를 통해 판매하고 구매하는 서비스

## 🧩기획 배경

- 관심 있는 물건이 먼저 예약이 잡혀 구매를 못하는 경우 발생
- 판매자와 구매자간의 가격 협상의 어려움
- 위와 같은 문제점을 해결하고자 경매 시스템을 통해 구매 결정

## 🎈해결 컨셉

- 경매 사이트는 사용자들이 다양한 물품에 대해 자유롭게 입찰할 수 있는 환경을 제공.
- 이 시스템을 통해 판매자는 복잡한 가격 협상 없이 최고 입찰가에 물품을 판매할 수 있으며, 구매자는 자신이 원하는 가격에 물품을 입찰할 수 있음.

## 🗝기대 효과

- 경매를 통한 판매자, 구매자간 합리적인 거래 가능
- 경매라는 공정한 시스템을 통해 모든 참가자에게 원하는 물품을 구매할 수 있는 기회 제공

## 🛠기술 스펙

- **회원가입 / 로그인**
    - **회원가입**: 아이디, 이메일과 비밀번호를 사용하여 계정을 생성하며, 이메일 인증을 통해 계정 활성화
    - **로그인**: 아이디, 비밀번호로 로그인 가능하며, 카카오, 네이버, 구글을 통한 소셜 로그인이 가능.
    - **아이디/비밀번호 찾기**: 이메일을 통해 아이디를 찾을 수 있으며 비밀번호의 경우 회원가입 시 작성한 이메일로 임시 비밀번호 발송 로그인 이후 비밀번호 수정.
    - **회원 정보 관리**: 사용자 정보 조회 및 수정 가능. 회원 탈퇴 기능 제공.
- **채팅**
    - **판매자와 소통**: 구매자는 판매자에게 상품에 대한 질문이나 보충 설명이 필요한 경우 채팅을 통해 소통.
    - **경매 종료 후 채팅방**: 경매 종료 후(낙찰시) 구매자와 판매자 간 상품 수령 방법 논의를 위한 채팅방이 자동 생성.
- **경매**
    - **경매 참여**: 모든 회원은 경매를 생성하고 참여할 수 있음.
    - **경매 관리**: 상세페이지에서 실시간 경매 기록을 확인 가능하며, 진행중인 경매는 수정 및 삭제가 불가.
    - **즉시 구매 기능**: 모든 경매는 즉시 구매가를 초과한 입찰이 불가능하며, 즉시 구매 시 경매가 종료.
    - **낙찰 및 알림**: 경매 종료 시 최고 입찰가의 구매자에게 낙찰되며, 판매자와 낙찰자에게 종료 알림이 발송.
        - 구매자의 구매 확정 시 거래 종료
        - 구매 확정은 일주일동안 유효하며 그 이후는 물건을 수령했다고 판단하여 자동 구매 확정 진행
    - **판매자 경매 등록**: 판매자는 상품 등록 시 상품 이름, 사진, 설명, 시작가, 즉시 구매가, 경매 기간, 수령 방법(만남 가능 여부와 지역 기재, 택배 가능 여부 및 착불/선불 선택)을 설정.
    - **입찰**: 구매자는 현재 입찰가보다 높은 금액으로 입찰할 수 있으며, 최소 입찰가 단위는 1,000원.
        
        - 입찰 시 포인트를 사용하며, 보유 포인트 이상의 금액으로 입찰할 수 없음.
        - 입찰 시 다른 경매에서 최고 입찰자로 존재하는 경우 현재 보유 포인트에서 최고 입찰가 금액만큼 제외하고 사용 가능
        
    - **포인트 관리**: 경매 종료 시 입찰자의 포인트가 소모되며, 구매자가 구매 확정 시 판매자에게 포인트가 지급.
- **Q&A 게시판**
    - **사용자 문의 및 답변**: 사용자들이 경매나 거래 관련 질문을 할 수 있는 공간을 제공하며, 게시물 작성 및 답글 기능을 통해 원활한 소통을 지원.
- **결제 / 포인트**
    - **포인트 충전 및 사용**: 입찰 전 포인트를 충전하여 사용하며, 포인트 100원당 현금 100원으로 충전.
    - 카카오페이 API를 사용하여 결제 시스템을 구현.

## 😎 조원 소개

<table>
  <tr>
    <th colspan="2" align="center">프로필</th>
    <th align="center">역할</th>
    <th align="center">작업 영역</th>
  </tr>
  <tr>
    <td align="center"><img src="https://avatars.githubusercontent.com/u/123534245?v=4" width="70"></td>
    <td>배진환(<a href="https://github.com/JinhwanB" target="_blank">@JinhwanB</a>)<br>Back-End</td>
    <td align="center">팀장</td>
    <td>경매 생성 및 종료, 경매 조회 및 hot5 경매 조회, 입찰 시스템, 입찰 내역 조회, 즉시 구매, 구매 확정, 판매 및 구매 내역 조회, Q&A CRUD</td>
  </tr>
  <tr>
    <td align="center"><img src="https://avatars.githubusercontent.com/u/108457670?v=4" width="70"></td>
    <td>최인영(<a href="https://github.com/choiinyoung13" target="_blank">@choiinyoung13</a>)<br>Front-End</td>
    <td align="center">팀원</td>
       <td>와이어 프레임 제작, 메인 페이지 구현, 채팅 페이지 및 실시간 채팅 구현, 최근 본 경매 모달 구현, 경매 리스트 페이지 구현, 로그인, 회원가입, 알림 모달 및 실시간 알림 구현 </td>
  </tr>
  <tr>
    <td align="center"><img src="https://avatars.githubusercontent.com/u/156155896?v=4" width="70"></td>
    <td>오동한(<a href="https://github.com/Oh-Donghan" target="_blank">@Oh-Donghan</a>)<br>Front-End</td>
    <td align="center">팀원</td>
   <td>상세페이지 레이아웃 구현, 입찰하기 및 즉시구매 구현, 마이페이지 레이아웃 구현, QnA 기능 구현, 이메일, 비밀번호 변경 구현, 회원 탈퇴 구현, MSW를 이용한 목데이터 생성</td>
  </tr>
  <tr>
    <td align="center"><img src="https://avatars.githubusercontent.com/u/102372626?v=4" width="70"></td>
    <td width="200">박민규(<a href="https://github.com/Cathunder" target="_blank">@Cathunder</a>)<br>Back-End</td>
    <td width="60" align="center">팀원</td>
    <td>포인트 결제, 포인트 잔액 및 충전/사용 내역 조회, 알림 기능 구현, 인프라 구축</td>
  </tr>
  <tr>
    <td align="center"><img src="https://github.com/user-attachments/assets/52095ae0-c76a-4cc4-8376-6a2d4843c3ee" width="70"></td>
    <td>엄석현(<a href="https://github.com/sh035" target="_blank">@sh035</a>)<br>Back-End</td>
    <td align="center">팀원</td>
    <td>채팅 기능 구현, 카테고리 조회, 소셜 로그인 구현 및 시큐리티 설계</td>
  </tr>
  <tr>
    <td align="center"><img src="https://avatars.githubusercontent.com/u/114427072?v=4" width="70"></td>
    <td>양승희(<a href="https://github.com/seungh22" target="_blank">@seungh22</a>)<br>Back-End</td>
    <td align="center">팀원</td>
    <td>회원가입, 로그인, 로그아웃, 이메일 및 비밀번호 변경, 아이디 찾기, 비밀번호 찾기</td>
  </tr>
</table>

<br>

## 아키텍처

![image](https://github.com/user-attachments/assets/dbf4aa63-2a41-47e7-958a-785cfb67d585)

## 사용 기술

### FE

![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)<br>
![NPM](https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white)<br>
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
<img src="https://img.shields.io/badge/typescript-239DAD?style=for-the-badge&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/recoli-3578E5?style=for-the-badge&logo=recoil&logoColor=white">
<img src="https://img.shields.io/badge/tanskquery-FF4154?style=for-the-badge&logo=reactquery&logoColor=white">
<img src="https://img.shields.io/badge/tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white">
![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)

### BE

![](https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white)
<br>
<img src="https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
<img src="https://img.shields.io/badge/spring boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
<img src="https://img.shields.io/badge/spring security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white">
<img src="https://img.shields.io/badge/websocket-010101?style=for-the-badge&logo=Socket.io&logoColor=white">
<img src="https://img.shields.io/badge/sse-171C36?style=for-the-badge&logo=sse&logoColor=white">
<img src="https://img.shields.io/badge/querydsl-0769AD?style=for-the-badge&logo=querydsl&logoColor=white">
<br>
<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
<img src="https://img.shields.io/badge/redis-FF4438?style=for-the-badge&logo=redis&logoColor=white">
<img src="https://img.shields.io/badge/h2-0854C1?style=for-the-badge&logo=h2&logoColor=white">
<br>
<img src="https://img.shields.io/badge/Amazon EC2-FF9900?style=for-the-badge&logo=Amazon EC2&logoColor=white">
<img src="https://img.shields.io/badge/amazons3-569A31?style=for-the-badge&logo=amazons3&logoColor=white">
<img src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
<img src="https://img.shields.io/badge/amazonroute53-8C4FFF?style=for-the-badge&logo=amazonroute53&logoColor=white">
<img src="https://img.shields.io/badge/awselasticloadbalancing-8C4FFF?style=for-the-badge&logo=awselasticloadbalancing&logoColor=white">
<img src="https://img.shields.io/badge/awssecretsmanager-DD344C?style=for-the-badge&logo=awssecretsmanager&logoColor=white">
<img src="https://img.shields.io/badge/githubactions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white">

## 와이어프레임

[와이어프레임](https://www.figma.com/design/npI8dmNSIYbq44YcCzX44A/wireFrame?node-id=0-1&node-type=CANVAS&t=dJDa2OJIuNsm8nH0-0)

## ERD

![중고 물품 경매 서비스 ERD.png](https://github.com/user-attachments/assets/cb11f9dd-bdf7-4668-86aa-ad0358329e24)
