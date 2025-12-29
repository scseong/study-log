# KAKAO TALK CLONE CODING

## About

- Kakao Talk 클론 코딩
  
- HTML/CSS 퍼블리싱 기본기 향상
  
- Github 이용하여 프로젝트 관리
  

## Demo

|     |     |     |     |
| --- | --- | --- | --- |
| 로그인 & 회원가입 | 친구 목록 | 채팅방 | 채팅 목록 |
| ![](https://user-images.githubusercontent.com/82589401/213380054-5442231e-378c-40eb-b82c-cbf7bb4a5a20.png) | ![](https://user-images.githubusercontent.com/82589401/213381063-508da66d-1ad3-48f9-b598-95929ccbe244.png) | ![](https://user-images.githubusercontent.com/82589401/213381114-2d3f7fa4-5e77-4cfa-aa29-9cccbfa11c37.png) | ![](https://user-images.githubusercontent.com/82589401/213381730-dedae4dc-8b9d-437e-802d-99718399b8c9.png) |
| 검색  | 더보기 | 설정  |     |
| ![](https://user-images.githubusercontent.com/82589401/213381740-1c6e636e-af85-462c-b1e7-a5bbb6cacc28.png) | ![](https://user-images.githubusercontent.com/82589401/213381751-ae2e0f6d-4987-437a-b3bd-aac620e21af7.png) | ![](https://user-images.githubusercontent.com/82589401/213381931-3bd52adb-c1cb-493e-807d-fe6a6d716a17.png) |     |

## Skills

- **HTML5 |** 웹 페이지와 내용을 구조화합니다. 웹페이지의 정보를 표현합니다.
  
- **CSS3 |** 스타일, 레이아웃 등 사용자에게 문서가 어떻게 보여질지 알려줍니다.
  

## Development focus

### (1) html, css 만으로 웹 애플리케이션 구현

```
📂 Directory Structure
│  .gitignore
│  chat.html
│  chats.html
│  find.html
│  friends.html
│  index.html
│  more.html
│  README.md
│  settings.html
└─css
    │  reset.css
    │  styles.css
    │  variables.css
    │
    ├─components
    │      alt-screen-header.css
    │      badge.css
    │      icon-row.css
    │      nav-bar.css
    │      screen-header.css
    │      status-bar.css
    │      user-component.css
    │
    └─screens
            chat.css
            find.css
            friends.css
            login.css
            more.css
            settings.css
```

### (2) 시멘틱 마크업

- 의미를 잘 전달 할 수 있도록 HTML 태그 문서를 작성
  
- HTML5 시멘틱 태그 활용
  

![semantic](https://user-images.githubusercontent.com/82589401/213413880-ccfd671a-50c6-4228-b961-d36e3aee1085.png)

### (3) CSS flexbox 레이아웃

레이아웃 배치 전용 기능으로 고안된 Flex의 강력하고 편리한 기능들을 활용

[Flexbox - Web 개발 학습하기 | MDN](https://developer.mozilla.org/ko/docs/Learn/CSS/CSS_layout/Flexbox)

### (4)효율적으로 CSS를 작성하기 위한 방법론 적용 - BEM

```html
<-- chats.html 일부 -->
<div class="user-component">
  <div class="user-component__column">
    <img
      src="https://t1.kakaocdn.net/kakaocorp/kakaocorp/admin/service/a85d0594017900001.jpg"
      alt="profile-img"
      class="user-component__avatar user-component__avatar--xl"
    />
    <div class="user-component__text">
      <h4 class="user-component__title">ChangSeong</h4>
      <h6 class="user-component__subtitle">😎</h6>
    </div>
  </div>
  <div class="user-component__column">
    <span class="user-component__time">21:22</span>
    <span class="badge">3</span>
  </div>
</div>
```

### (5) Github을 적극적으로 활용하며 개발하기

[이전에 정리했던 Github 협업하기 TIL](https://github.com/scseong/TIL/blob/main/2021/211126_TIL.md)

#### Issue, PR, Projects

프로젝트를 진행하며 기능 구현, 생기는 문제 등을 Issue로 작성하여 Projects와도 연동하여 작업 내용과 진행사항을 관리하였습니다. 커밋 메시지를 작성할 때도 Issue 번호를 명시하여 개발을 진행하였습니다.

(Issue와 PR 템플릿을 등록하여 활용)

![image](https://user-images.githubusercontent.com/82589401/213421558-d133d55a-faff-429e-8d70-01ffa1e50be1.png)

![image](https://user-images.githubusercontent.com/82589401/213415931-607a8492-adbd-4c57-8380-577d144191a7.png)

![image](https://user-images.githubusercontent.com/82589401/213427173-e71243e6-2c4e-41e8-9903-8ce7b9b0cbce.png)

#### 깃 브랜치 전략을 적용

**git-flow**

5가지의 브랜치를 이용해 운영하는 브랜치 전략

- **main**: 배포 가능한 브랜치
  
- **develop**: 개발한 기능이 모여있는 브랜치
  
- **feature**: 기능을 개발하는 브랜치 (develop 에서 분기)
  
- **release**: QA(품질검사)를 하기위한 브랜치 (출시 준비)
  
- **hotfix**: main 브랜치에 발생한 버그를 긴급수정하는 브랜치
