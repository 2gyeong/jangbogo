# 똑똑한 소비의 시작 - 카트왕 장보고 🛒

<br>
<br>23. 03. 14 - 23. 04. 09</br>

[![Video Label](https://img.youtube.com/vi/fY7ZD8Zx0Qg/0.jpg)](https://www.youtube.com/watch?v=fY7ZD8Zx0Qg)


<h3>프로젝트 소개</h3>
<hr>

- 농수산물 가격 변동을 그래프로 볼 수 있습니다.<br>
- 네이버 검색 API를 통해 쇼핑 사이트를 제공합니다.<br>
- 커뮤니티 게시판을 통하여 회원간 정보 공유 및 친목 도모를 할 수 있습니다.<br>


<h3>개발 환경</h3>
<hr>

<div>
<img src="https://img.shields.io/badge/java 11-007396?style=for-the-badge&logo=java&logoColor=white">
<img src="https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
<img src="https://img.shields.io/badge/spring security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white">
<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> 
</div>

<div>
<img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black"> 
<img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
<img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> 
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> 
  <img src="https://img.shields.io/badge/jquery-0769AD?style=for-the-badge&logo=jquery&logoColor=white">
</div>
<div>
<img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">
<img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white">
</div>


<h3>프로젝트 구조</h3>
<hr>

```
📦com
 ┗ 📂jangbogo
 ┃ ┣ 📂advice
 ┃ ┃ ┣ 📂assertThat
 ┃ ┃ ┃ ┗ 📜DefaultAssert.java
 ┃ ┃ ┣ 📂error
 ┃ ┃ ┃ ┣ 📜DefaultAuthenticationException.java
 ┃ ┃ ┃ ┣ 📜DefaultException.java
 ┃ ┃ ┃ ┣ 📜DefaultNullPointerException.java
 ┃ ┃ ┃ ┗ 📜InvalidParameterException.java
 ┃ ┃ ┣ 📂payload
 ┃ ┃ ┃ ┣ 📜ErrorCode.java
 ┃ ┃ ┃ ┗ 📜ErrorResponse.java
 ┃ ┃ ┣ 📜ApiControllerAdvice.java
 ┃ ┃ ┗ 📜MemberNotFoundException.java
 ┃ ┣ 📂config
 ┃ ┃ ┣ 📂handler
 ┃ ┃ ┃ ┣ 📜CustomSimpleUrlAuthenticationFailureHandler.java
 ┃ ┃ ┃ ┗ 📜CustomSimpleUrlAuthenticationSuccessHandler.java
 ┃ ┃ ┣ 📂security
 ┃ ┃ ┃ ┣ 📂auth
 ┃ ┃ ┃ ┃ ┣ 📂company
 ┃ ┃ ┃ ┃ ┃ ┣ 📜Kakao.java
 ┃ ┃ ┃ ┃ ┃ ┗ 📜Naver.java
 ┃ ┃ ┃ ┃ ┣ 📜Oauth2UserInfo.java
 ┃ ┃ ┃ ┃ ┗ 📜Oauth2UserInfoFactory.java
 ┃ ┃ ┃ ┣ 📂docs
 ┃ ┃ ┃ ┃ ┗ 📜OpenApiConfig.java
 ┃ ┃ ┃ ┣ 📂token
 ┃ ┃ ┃ ┃ ┣ 📜CurrentUser.java
 ┃ ┃ ┃ ┃ ┣ 📜CustomAuthenticationEntryPoint.java
 ┃ ┃ ┃ ┃ ┣ 📜CustomOncePerRequestFilter.java
 ┃ ┃ ┃ ┃ ┗ 📜UserPrincipal.java
 ┃ ┃ ┃ ┣ 📂util
 ┃ ┃ ┃ ┃ ┗ 📜CustomCookie.java
 ┃ ┃ ┃ ┣ 📜OAuth2Config.java
 ┃ ┃ ┃ ┣ 📜SecurityConfig.java
 ┃ ┃ ┃ ┗ 📜WebMvcConfig.java
 ┃ ┃ ┗ 📜AuditConfig.java
 ┃ ┣ 📂constant
 ┃ ┃ ┗ 📜Role.java
 ┃ ┣ 📂controller
 ┃ ┃ ┣ 📜AnswerController.java
 ┃ ┃ ┣ 📜AuthController.java
 ┃ ┃ ┣ 📜MessageController.java
 ┃ ┃ ┣ 📜PriceController.java
 ┃ ┃ ┣ 📜PriceInfoController.java
 ┃ ┃ ┣ 📜QuestionController.java
 ┃ ┃ ┣ 📜SearchRequestController.java
 ┃ ┃ ┗ 📜ZzimController.java
 ┃ ┣ 📂domain
 ┃ ┃ ┣ 📂Board
 ┃ ┃ ┃ ┣ 📜Answer.java
 ┃ ┃ ┃ ┣ 📜Board.java
 ┃ ┃ ┃ ┗ 📜Question.java
 ┃ ┃ ┣ 📂common
 ┃ ┃ ┃ ┣ 📜BaseEntity.java
 ┃ ┃ ┃ ┗ 📜BaseTimeEntity.java
 ┃ ┃ ┣ 📂member
 ┃ ┃ ┃ ┣ 📂entity
 ┃ ┃ ┃ ┃ ┣ 📜Member.java
 ┃ ┃ ┃ ┃ ┣ 📜Provider.java
 ┃ ┃ ┃ ┃ ┣ 📜Role.java
 ┃ ┃ ┃ ┃ ┗ 📜Token.java
 ┃ ┃ ┃ ┗ 📂mapping
 ┃ ┃ ┃ ┃ ┗ 📜TokenMapping.java
 ┃ ┃ ┣ 📂product
 ┃ ┃ ┃ ┣ 📜Product.java
 ┃ ┃ ┃ ┗ 📜Zzim.java
 ┃ ┃ ┣ 📜DirectMessage.java
 ┃ ┃ ┣ 📜Favorite.java
 ┃ ┃ ┗ 📜PriceInfo.java
 ┃ ┣ 📂dto
 ┃ ┃ ┣ 📜AnswerDto.java
 ┃ ┃ ┣ 📜ItemDto.java
 ┃ ┃ ┣ 📜PriceDto.java
 ┃ ┃ ┣ 📜PriceInfoDTO.java
 ┃ ┃ ┣ 📜ProductRequestDto.java
 ┃ ┃ ┣ 📜QuestionDto.java
 ┃ ┃ ┗ 📜ZzimDto.java
 ┃ ┣ 📂exeption
 ┃ ┃ ┣ 📜DataNotFoundException.java
 ┃ ┃ ┣ 📜MemberNotEqualsException.java
 ┃ ┃ ┣ 📜MemberNotFoundException.java
 ┃ ┃ ┗ 📜MessageNotFoundException.java
 ┃ ┣ 📂payload
 ┃ ┃ ┣ 📂request
 ┃ ┃ ┃ ┣ 📂auth
 ┃ ┃ ┃ ┃ ┣ 📜ChangePasswordRequest.java
 ┃ ┃ ┃ ┃ ┣ 📜RefreshTokenRequest.java
 ┃ ┃ ┃ ┃ ┣ 📜SignInRequest.java
 ┃ ┃ ┃ ┃ ┣ 📜SignUpRequest.java
 ┃ ┃ ┃ ┃ ┗ 📜UpdateRequest.java
 ┃ ┃ ┃ ┗ 📂message
 ┃ ┃ ┃ ┃ ┣ 📜MessageCreateRequest.java
 ┃ ┃ ┃ ┃ ┗ 📜MessageDto.java
 ┃ ┃ ┗ 📂response
 ┃ ┃ ┃ ┣ 📂DM
 ┃ ┃ ┃ ┃ ┣ 📜Failure.java
 ┃ ┃ ┃ ┃ ┣ 📜Response.java
 ┃ ┃ ┃ ┃ ┣ 📜Result.java
 ┃ ┃ ┃ ┃ ┗ 📜Success.java
 ┃ ┃ ┃ ┣ 📜ApiResponse.java
 ┃ ┃ ┃ ┣ 📜AuthResponse.java
 ┃ ┃ ┃ ┣ 📜MailResponse.java
 ┃ ┃ ┃ ┗ 📜Message.java
 ┃ ┣ 📂repository
 ┃ ┃ ┣ 📂auth
 ┃ ┃ ┃ ┣ 📜CustomAuthorizationRequestRepository.java
 ┃ ┃ ┃ ┗ 📜TokenRepository.java
 ┃ ┃ ┣ 📜AnswerRepository.java
 ┃ ┃ ┣ 📜BoardRepository.java
 ┃ ┃ ┣ 📜MemberRepository.java
 ┃ ┃ ┣ 📜MessageRepository.java
 ┃ ┃ ┣ 📜PriceInfoRepository.java
 ┃ ┃ ┣ 📜ProductRepository.java
 ┃ ┃ ┣ 📜QuestionRepository.java
 ┃ ┃ ┗ 📜ZzimRepository.java
 ┃ ┣ 📂service
 ┃ ┃ ┣ 📂auth
 ┃ ┃ ┃ ┣ 📜AuthService.java
 ┃ ┃ ┃ ┣ 📜CustomDefaultOAuth2UserService.java
 ┃ ┃ ┃ ┣ 📜CustomTokenProviderService.java
 ┃ ┃ ┃ ┗ 📜CustomUserDetailsService.java
 ┃ ┃ ┣ 📜AnswerService.java
 ┃ ┃ ┣ 📜FileService.java
 ┃ ┃ ┣ 📜MailService.java
 ┃ ┃ ┣ 📜MemberService.java
 ┃ ┃ ┣ 📜MessageService.java
 ┃ ┃ ┣ 📜PriceInfoService.java
 ┃ ┃ ┣ 📜QuestionService.java
 ┃ ┃ ┗ 📜ZzimService.java
 ┃ ┣ 📂util
 ┃ ┃ ┣ 📜NaverShopSearch.java
 ┃ ┃ ┗ 📜PriceInfoJsonParser.java
 ┃ ┗ 📜JangbogoApplication.java

```

<h3>역할 분담</h3>
<hr>

- 김이경 : 메인화면 농수산물 가격 조회</br>
- 전은비 : 회원가입, 로그인(kakao, naver), 회원정보 수정, 회원 탈퇴</br>
- 황인재 : 네이버 검색 API를 통한 상품 조회, 상품 정렬, 상품 찜하기 및 삭제</br>
- 이효진, 지혁진 : 커뮤니티 게시판 지역별 분류, 게시판 글 쓰기, 글 수정 및 삭제, 게시글 추천 및 취소</br>
- 김지수 : 회원 간 쪽지 보내기, 보낸 쪽지 삭제, 받은 쪽지 삭제, 보낸 쪽지 및 받은 쪽지 확인</br>
</br>

