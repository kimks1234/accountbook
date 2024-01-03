# 가계부 팀 프로젝트 
## 프로젝트 개요
이번 프로젝트는 가계부 앱을 만드는 프로젝트로 프론트 엔드와 백 엔드 그리고 데이터베이스의 기술을 이용해 작업을 하였다. <br>
이 중에서 저는 프론트 엔드 기능 개발 담당과 MongoDB를 이용해서 로그인할 때 서버와 연동되는 백 엔드 부분을 도맡아 했다.

## 기획의도 & 목표
이 프로 젝트의 기획의도는 MongoDB를 이용해 회원가입과 로그인을 구현하고 가계부 앱을 통해 실제 예산관리를 하면서 지출을 줄여보자는 의도를 가지고 있다. 

### 목표
*	리액트 경험을 늘리고 사용 기술 향상
*	앱의 가독성을 위한 기본적인 UI/UX 디자인을 파악
* 팀원 들과의 협업을 통해 커뮤니케이션 능력 향상
*	MongoDB와 express를 이용해 로그인/회원가입을 구현
  
## 프로젝트 작업 순서
1. 팀원과 자기 소개 후 앱 선정과 역할 분담
2. 워크플로우와 기능적 요구사항 분석
3. 디렉토리 구조 설정
4. git organization 레파지토리 생성
5. 리액트 앱 생성
6. 앱 기능 만들기
7. 앱 CSS 퍼블리싱
8. 가계부 회원 가입 / 로그인 MongoDB에 연결
9. PPT 발표

## 사용기술
Tool : GitHub , Visual Studio Code  <br>
웹 화면:  CSS, JavaScript<br>
데이터베이스: MongoDB<br>
사용 라이브러리: react , react-calendar, react-router-dom, rechart.js , express.js<br>

## 담당업무
* 프로젝트 리더
* 주요기능 담당
* 로그인/회원가입 MongoDB 연결

## 프로젝트 내용
### 기능적 요구 사항
![기능적요구사항](https://github.com/kimks1234/accountBook/assets/142865411/b92088f1-eb25-417a-9acc-7098f9a88da4)

### 워크플로우
![1703225689702-62aa3ee4-fa60-407b-a569-11da06bb2740_1](https://github.com/kimks1234/accountBook/assets/142865411/a46dbde5-fe23-4a40-9e23-c278b1b12f96)

### 디렉토리 구조
![디렉토리구조](https://github.com/kimks1234/accountBook/assets/142865411/bad94bbf-01d7-4c10-a011-7ca3512184ce)

### 페이지 구성
![가계부](https://github.com/kimks1234/accountBook/assets/142865411/28f63a92-57e5-4c17-893c-0b8ad705fbd3)

### 문제 및 해결
* 상황: 깃 허브 페이지에 결과물을 올렸는데 앱 안의 내용이 하나도 보이지 않음 <br>
* 문제확인: 라우터를 설정하면 앱 안의 내용이 보이지 않을 수 있다는 사실을 깨달음 <br>
* 해결: 프론트엔드 최상위 index.js 앱을 감싸고 있는 BrouserRouter 에 <br>
```<BrowserRouter basename={process.env.PUBLIC_URL}>``` 코드를 작성하고 다시 push와npm run build를 하여 문제를 해결함 <br>

* 상황: 등록페이지 라우터에서 메인 라우터로 데이터가 전송이 되어야 하는데 저장을 눌러도 데이터가 전송이 안되는 상황 <br>
* 해결: 배운 것 중에 Context API가 생각이나 context를 통해 데이터상태관리를 하여 데이터를 다른 라우터에도 공유가 되게 함

