## 제작 기간 & 참여 인원
* 22.7.14 ~ 22.8.16  
* 4인 팀 프로젝트
* 맡은 역할 : 리드 developer / back-end developer

## Stack
* Language : Python, Javascript
* Framework : Django, DRF
* Database : MySQL
* Infra : AWS EC2, AWS S3, Docker

## Layout
![](https://velog.velcdn.com/images/soyoyun/post/5132721f-4b6d-47ce-a4cd-9bd12880bf8d/image.png)

## [ERD](https://www.erdcloud.com/d/EL9ztjydoLhqhysPe)
![image](https://user-images.githubusercontent.com/90381057/186103025-070baeb8-083d-4394-9153-207b4751c940.png)

### **API 설계**
[article](https://documenter.getpostman.com/view/16204656/VUquLFrn#intro)  
[community](https://documenter.getpostman.com/view/16204656/VUquLFw9)  
[noticeboard](https://documenter.getpostman.com/view/16204656/VUquLajN)  
[user](https://documenter.getpostman.com/view/16204656/VUquLajQ)  


### **프로젝트 진행 순서**

<details>
<summary>보기</summary>
<div markdown="1">

> 발제 → 프로젝트 Notion page 개설 → 주제 브레인스토밍 → 주제선정 → GitHub repository 개설 → Figma 이용해 레이아웃 제작 → 역할분담 및 마감기한 구체화 → 중간 중간 회의 및 팀 내 피드백 → 최종 피드백 → 완성

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
