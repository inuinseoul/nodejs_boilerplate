# nodejs_boilerplate
This is made for node.js boilerplate production.
(from [inflearn jhonahn's lecture](https://www.inflearn.com/course/%EB%94%B0%EB%9D%BC%ED%95%98%EB%A9%B0-%EB%B0%B0%EC%9A%B0%EB%8A%94-%EB%85%B8%EB%93%9C-%EB%A6%AC%EC%95%A1%ED%8A%B8-%EA%B8%B0%EB%B3%B8))

## Library

**server**

- node.js
- mongoDB (mongoose)
- express
- body-parser
- cookie-parser
- bcrypt
- jsonwebtoken

**client**

- react (react-router-dom)
- axios
- http-proxy-middleware
- Antd CSS Framework
- redux (react-redux, redux-promise, redux-thunk)

## Study Points

**server**

- node.js를 통해 기본 백엔드 구성
- mongoose와 mongoDB를 node.js 서버와 연결
- cookie, jwt, db 등의 활용으로 기본적인 인증 구현
- client와 server간의 기본적 관계 및 데이터 Flow 파악

**client**

- React를 사용해 기본 프론트엔드 구성
- Proxy server 활용으로 CROS 이슈 해결방법
- Concurrently를 이용해 프론트, 백 서버 한번에 켜기
- Redux의 data flow(unidirectional data flow) 및 기초 활용방법
- React hooks 활용으로 Functional Component에서 state 사용
- auth를 체크해 권한마다 페이지 접근을 제한하는 방법

## About Client Folder Structure

- _actions, _reduce : Redux를 위한 폴더들
- componets/views : page 구성
- componets/views/Sections : page와 관련된 css 및 component 구성
- App.js : Routing 관련 일 처리
- Config.js : 환경 변수 등의 작업 처리
- hoc : Higher Order Component의 약자. 특정 component에 들어가기 전 선행되어 실행되는 component (ex. auth)
- utils : 여러 곳에서 쓰는 것을 넣어서 어디서든 사용할 수 있도록 처리

## ETC

- Babel : 하위 버전의 Javascript만을 지원하는 브라우저를 위해 이를 변환해주는 역할을 함
- CORS 정책 : Cross-Origin Resource Sharing 정책으로, 서로 다른 origin간의 resource sharing을 제한하는 것 (보안의 목적)
- Proxy server : 방화벽 기능 / 웹 필터 기능 / 캐쉬 데이터, 공유 데이터 제공 등의 기능을 제공하는 중간 서버
- prps : 변하지 않는 부모 컴포넌트로부터 받는 값들로 수정이 불가능하다.
- state : 부모로부터 받는 것이 아닌 컴포넌트 안에서 데이터를 전달하는 것으로 수정이 가능하다. (state가 변하면 re-render 수행) 
- Redux : Javascript의 state 관리 라이브러리 (일종의 state 저장소같은 느낌)
- action : 사용자가 수행하는 행위에 대한 정보가 담겨있는 객체(object)
- reducer : previousState와 action object를 받아 nextState를 리턴한다
- store : 어플리케이션 전체의 state을 감싸주는 역할. 자체 메소드를 보유하고 있어 이를 통해 state를 관리할 수 있다.
- React Component : class component vs functional component
- React hooks : functional component에서 class component의 기능을 사용하기 위해 개발된 것
