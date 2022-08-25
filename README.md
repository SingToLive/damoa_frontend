# Project Damoa

## 목차
1. 프로젝트 소개  
2. 팀 구성  
3. 기술 스텍 및 라이브러리  
4. 주요 기능  
5. Troubleshooting  
6. 유저 피드백 및 개선 사항

## 📄 프로젝트 소개
프로젝트 다모아는 인가된 인원에 대해 자유롭게 커뮤니티를 형성할 수 있는 사이트입니다. 기업, 커뮤니티, 작게는 개인까지 소통을 이어나갈 수 있으며 운동, IT, 음식 등 다양한 주제로 소통방을 만들 수 있습니다. 글 또한 고민, 질문, 자랑 등 자유로운 얘기를 할 수 있습니다.    

### ⏲ 개발 기간 : 2022.7.14 ~ 2022.8.16

### 홈페이지  (현재는 닫힌 상태입니다.)

### 소개 영상  [youtube](https://youtu.be/6c7Q82DfTAU)

### Github  [Front-end](https://github.com/Reinforcement-succeeded/damoa_frontend)

### Github  [Back-end](https://github.com/Reinforcement-succeeded/damoa_backend)

## 🧑 팀 구성 
* 4인 팀 프로젝트  <br>
* 맡은 역할 : lead developer / back-end developer / front-end developer

<table>
  <tr>
    <td align="center"><strong>구분</strong></td>
    <td align="center"><strong>Back-end</strong></td>
    <td align="center"><strong>Front-end</strong></td>
    <td align="center"><strong>Designer</strong></td>
    <td align="center"><strong>AI Engineer</strong></td>	  
  </tr>
  <tr>
    <td align="center"><strong>메인페이지</strong></td>
    <td align="center">이승태</td>
    <td align="center">이승태</td>
    <td align="center">이승태</td>
    <td rowspan="5" align="center">전진영</td>
  </tr>
  <tr>
    <td align="center"><strong>마이페이지</strong></td>
    <td align="center">이승태</td>
    <td align="center">이승태</td>
    <td align="center">이승태</td>
  </tr>
  <tr>
    <td align="center"><strong>로그인 페이지</strong></td>
    <td align="center">이승태</td>
    <td align="center">이승태</td>
    <td align="center">이승태</br>전진영</td>
  </tr>
  <tr>
    <td align="center"><strong>회원가입 페이지</strong></td>
    <td align="center">이승태</td>
    <td align="center">이승태</td>
    <td align="center">이승태</br>전진영</td>
  </tr>
  <tr>
    <td align="center"><strong>커뮤니티 페이지</strong></td>
    <td align="center">이승태</br>윤가현</br>김민재</td>
    <td align="center">이승태</br>윤가현</br>김민재</td>
    <td align="center">이승태</br>윤가현</br>김민재</td>
  </tr>
</table>

## ✨ Stack
* Language : Python, Javascript
* Framework : Django, DRF
* Database : MySQL
* Infra : AWS EC2, AWS S3, Docker

## 🕹 주요 기능
### 로그인 / 회원가입
* JWT 토큰 방식으로 구현
* Local Storage에 저장
* 각 페이지마다 접속시 refresh token을 받게 설정
* 아이디를 고유값으로 지정하여 중복 방지

### 메인 페이지
* 로그인 유무에 따라 추천 커뮤니티 변경
    * 추천 커뮤니티는 무조건 공개 커뮤니티에 대해서만 제공
* 커뮤니티 별 하루 접속자 수 순위표 제공
* 가입되지 않은 커뮤니티에 가입 요청 / 요청 취소 가능
* 커뮤니티 카드를 누를시 해당 커뮤니티로 이동
    * 단 가입되지 않은 커뮤니티는 접속 불가능
* 커뮤니티 생성
    * 커뮤니티 생성자는 관리자로 자동 설정

### 마이 페이지
* 비밀번호 변경 가능
* 가입된 커뮤니티 관리
* 작성한 글 관리(이동은 미구현)
* 작성한 댓글 관리(이동은 미구현)
* 유저->커뮤니티 가입 요청 결과 조회 / 요청 철회 / 요청 삭제
* 커뮤니티->유저 가입 요청 승락 / 요청 거절

### 커뮤니티 페이지
* 게시판 생성
   * 생성자는 게시판 관리자도 자동 설정
* 게시글 작성
   * Quill Library로 게시글 작성 기능 구현
   * 게시글에서 이미지 업로드 가능
   * 파일 업로드 가능
   * 게시글 제목, 내용중 하나라도 누락이 있을시 작성 불가능
* 게시글 수정
   * 게시글 제목, 내용중 하나라도 누락이 있을시 작성 불가능
* 댓글 작성
   * 생성시 날짜, 아이디 노출
   * 시간순으로 배치
   * 내용이 없으면 작성 불가능

## ⚙ [ERD](https://www.erdcloud.com/d/EL9ztjydoLhqhysPe)
![image](https://user-images.githubusercontent.com/90381057/186103025-070baeb8-083d-4394-9153-207b4751c940.png)

## 🚀 **API 설계**
[article](https://documenter.getpostman.com/view/16204656/VUquLFrn#intro)  
[community](https://documenter.getpostman.com/view/16204656/VUquLFw9)  
[noticeboard](https://documenter.getpostman.com/view/16204656/VUquLajN)  
[user](https://documenter.getpostman.com/view/16204656/VUquLajQ)  

## 🗺 Layout
![Group 26](https://user-images.githubusercontent.com/90381057/186547234-04a9537b-2f48-4a3d-903b-bed3f7b3ba8d.png)

## **프로젝트 진행 순서**
발제 → 프로젝트 Notion page 개설 → 주제 브레인스토밍 → 주제선정 → GitHub repository 개설 → Figma 이용해 레이아웃 제작 → 역할분담 및 마감기한 구체화 → 중간 중간 회의 및 팀 내 피드백 → 최종 피드백 → 완성


## 주제

**부트캠프 및 온라인 스터디 커뮤니티**<br>
**테스터 : 내일배움캠프 인원**<br>
확장성 : 부트캠프 수료자, 온라인 스터디 커뮤니티 개설을 원하는 사람들을 위한 서비스<br><br>

**사이트에서 구현해볼 기능**

-   추천, 댓글 기능 외 다양한 기능 (추후 계속 추가해볼 예정)
-   태그기능 -> #python #django 카테고리별 보기

-   **팀 내 약속 [소통]**
	-   자리비울일 있거나 얘기 나눌때 Gather, Slack으로 소통
	-   오후 5시, 3시(5시에 일정이 있을경우) 작업 진행도 팀원과 공유하기

-   **팀 내 약속 [기능]**

    -   개인이 맡은 기능 작업 후 **daily로 main branch에 머지**
    -   Github Readme, Wiki 계속 업데이트
    -   미리 정해둔 **폴더**, **파일 경로설정**, 커밋메세지 컨벤션 지키기
    -   git add 시 파일 하나씩 올리면서 커밋메세지에 세부사항 적기
    -   git issue 이용해 할 일 구체화하고 기록해 작업 효율성 높이기
    -   가상환경, 인터프리터 통일
        -   python 3.9.12, django 4.0.4
    -   커밋메세지 컨벤션
        -   MOD : modify한 내용
        -   ENH : enhancement한 내용
        -   ADD : add한 내용
        -   DEL : delete한 내용
        -   MOV : move한 내용
        -   MOD & MOV : modify한 내용 & move한 내용
    -   .gitignore로 필요없는 파일은 업로드 시키지 않기
    -   결과값 신뢰도를 높이기 위한 커스텀 데이터 생성

-   **팀명과 팀원: 9000(6조) (윤가현[팀장], 김민재, 전진영, 이승태)**
-   **역할 분담** - **AI 모델 제작 : 진영**
    -   AI 자연어 : 불용어 + 감정평가, 이미지 처리 <br><br>
-   **백엔드, 프론트 담당 : 승태, 민재, 가현, 진영**
    - 로그인및 회원가입, 메인페이지, 마이페이지, 커뮤니티페이지 - 승태 / 커뮤니티페이지 분업- 민재, 가현<br><br>
-   **발표자 및 영상촬영**
    -   **발표자 : 승태**
    -   **영상촬영 : 승태**<br>
