## 제작 기간 & 참여 인원
* 22.7.14 ~ 22.8.16  
* 팀 프로젝트
* 맡은 역할 : back-end developer

## Stack
* Language : Python, Javascript
* Framework : Django, DRF, Flask
* Database : MySQL
* Infra : AWS EC2, AWS S3, Docker

## Layout
![](https://velog.velcdn.com/images/soyoyun/post/5132721f-4b6d-47ce-a4cd-9bd12880bf8d/image.png)

## [ERD](https://www.erdcloud.com/d/EL9ztjydoLhqhysPe)
![image](https://user-images.githubusercontent.com/90381057/186103025-070baeb8-083d-4394-9153-207b4751c940.png)


### **프로젝트 진행 순서**

<details>
<summary>보기</summary>
<div markdown="1">

> 발제 → 프로젝트 Notion page 개설 → 주제 브레인스토밍 → 주제선정 → GitHub repository 개설 → Figma 이용해 레이아웃 제작 → 역할분담 및 마감기한 구체화 → 중간 중간 회의 및 팀 내 피드백 → 최종 피드백 → 완성

</div>
</details>

---

### **브레인스토밍**

<details>
<summary>🧠 주제 브레인스토밍 보기</summary>
<div markdown="1">

```
   가현

   도서 검색
   - 전국에 있는 도서관에서 검색할 수 있는
   - 대출 현황
   - 전체 하루 대출, 반납량

   여행지 추천
   - 서울 놀러갈 곳/ 제주도 먹거리, 볼거리
   - 위와 같은 내용을 모아준다
   - 데이트 어플같은거 보면은 서울시에서 무슨무슨구에는 어떤 데이트 장소가 있어서
   어떤 취향이시면 추천합니다

   - 의식주 관련 사이트
   - 미술관 모아주는 사이트

   진영
   여행추천 사이트

   승태
   운동 사이트
   - 자리 났을 때 알려주는(잔여백신 같은 느낌)

   민재
   게임추천 사이트
   - 게임 태그(rpg, console)
   - 순서대로 평점, 다운로드 수

   영화 장면
   - 사진을 기반으로 출처를 찾아주는
   - 여기가 어딘지 알려주는
   - 데이터셋을 만들어야할거 같은 느낌이

   미술과 명화 알려주기
   - 인물 정보
   - 전시되어 있는 위치
   - 같은 작가의 작품

   우진
   스파르타 인원끼리 끈끈해지자, 스파르타 커뮤니티
```

</div>
</details>

<details>
<summary>🧠 서비스에 들어가야할 필수 카테고리 브레인스토밍 보기</summary>
<div markdown="1">

```
가현
- 메인 화면
	- 바로가기 유저가 생성 가능?
		- 공식(스파르타) 사이트 바로가기
		- 사이트 이벤트 바로가기
		- 스파르타 전시회 바로가기

- 자유 정보 게시판
(이 안에 유저가 python, django 등 정보 올릴 게시판 자율적으로 생성 가능, 이용순 혹은 가나다순으로 정렬, 찜기능시 맨위로 게시판 올리기 가능)

- 홍보 게시판
- 질문 게시판
- 출첵 게시판

진영
- 질문방(스택별)
- 잡담방(카테고리별 유저가 자유롭게)
- 잡담방-익명 질문방-실명

승태
- DC처럼 처음에는 모든 갤러리(커뮤니티)가 다 보여지게 단, 갤러리 접근은 인증이 되어야만 가능
- 사용자의 필요에 따라 로그인 후 첫 시작 화면이 모든 갤러리가 보이는 메인 화면 또는 자신이 설정한 갤러리 메인 화면이 될 수 있음
- 갤러리의 생성은 자유롭게 가능?

- 메인
	- 갤러리
	- 이벤트
	-

- 갤러리
	- 자유게시판
	- 익명게시판

민재
- 메인 화면
	ㄴ 자유 게시판
	ㄴ 질문 게시판
	ㄴ 건의 게시판
	ㄴ 프로젝트 소개 게시판
	ㄴ 강의 추천 게시판
		 ㄴpython 강의 추천
			 django 강의 추천
	     등등
	ㄴ 취미 게시판
	ㄴ 여행 게시판
	ㄴ 팀 모집 게시판
	ㄴ 애완동물 자랑 게시판**

```

</div>
</details>

---

### ▶️ 최종주제

**부트캠프 및 온라인 스터디 커뮤니티**<br>
**테스터 : 내일배움캠프 인원**<br>
확장성 : 부트캠프 수료자, 온라인 스터디 커뮤니티 개설을 원하는 사람들을 위한 서비스<br><br>

**사이트에서 구현해볼 기능**

-   추천, 댓글 기능 외 다양한 기능 (추후 계속 추가해볼 예정)
-   태그기능 -> #python #django 카테고리별 보기

---

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

    ***

-   **팀명과 팀원: 9000(6조) (윤가현[팀장], 김민재, 전진영, 이승태)**
-   **1차 개발 기간 : 22.07.14.목 ~ 22.07.21.목 오후 5:00 마감**
-   **역할 분담** - **AI 모델 제작 : 진영**
    -   AI 자연어 : 불용어 + 감정평가, 이미지 처리 <br><br>
-   **백엔드, 프론트 담당 : 승태, 민재, 가현, 진영**
    -   백엔드 : 로그인및 회원가입, 메인페이지 - 승태 / 커뮤니티페이지 분업- 민재, 가현<br><br>
-   **발표자 및 영상촬영**
    -   **발표자 : 승태**
    -   **영상촬영 : 진영**<br>

---

### **API 설계**

![](https://velog.velcdn.com/images/soyoyun/post/5cc5499c-a6f7-41c0-9e9c-080e83406532/image.png)

### **페이지 레이아웃**



### **페이지 세부 레이아웃**

**로그인 - 로그아웃**
![](https://velog.velcdn.com/images/soyoyun/post/55635918-2a92-43b4-8d5a-73415a35f1b7/image.png)

**메인페이지**
![](https://velog.velcdn.com/images/soyoyun/post/717de1b5-73dc-47ce-95ec-04a172cea770/image.png)

**인증 필요할경우**
![](https://velog.velcdn.com/images/soyoyun/post/fc1fe873-ea44-4c38-9a29-a63f6f288b84/image.png)

**게시판 설계도**
![](https://velog.velcdn.com/images/soyoyun/post/bbda55c5-2a69-49fd-8b3f-45ea7f0caae2/image.png)

**관리자 페이지에는 왼쪽에 관리항목이 추가되어 보입니다.<br>
커뮤니티 관리자는 글 승인/거절 페이지에 접근할 수 있습니다.**
![](https://velog.velcdn.com/images/soyoyun/post/352c554d-98e8-4f9c-88ef-5b9ae75ebc82/image.png)

### **DB설계**

![](https://velog.velcdn.com/images/soyoyun/post/d55cf6c0-2f4e-454b-812a-8ec6384ce48c/image.png)
