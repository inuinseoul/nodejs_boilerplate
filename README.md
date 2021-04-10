# nodejs_boilerplate
This is made for node.js boilerplate production.

server 

- node.js
- mongoDB (mongoose)
- express
- body-parser
- cookie-parser
- bcrypt
- jsonwebtoken

client

- react (react-router-dom)
- axios
- http-proxy-middleware

## Study Points

server

- study point1 👉 node.js를 통해 기본 백엔드 구성
- sutdy point2 👉 mongoose와 mongoDB를 node.js 서버와 연결
- study point3 👉 cookie, jwt, db 등의 활용으로 기본적인 인증 구현
- study point4 👉 client와 server간의 기본적 관계 및 데이터 Flow 파악

client

- study point1 👉 React를 사용해 기본 프론트엔드 구성
- study point2 👉 Proxy server 활용으로 CROS 이슈 해결방법

## About Client Folder Structure

- _actions, _reduce : Redux를 위한 폴더들
- componets/views : page 구성
- componets/views/Sections : page와 관련된 css 및 component 구성
- App.js : Routing 관련 일 처리
- Config.js : 환경 변수 등의 작업 처리
- hoc : Higher Order Component의 약자. 특정 component에 들어가기 전 선행되어 실행되는 component (ex. auth)
- utils : 여러 곳에서 쓰는 것을 넣어서 어디서든 사용할 수 있도록 처리

## ETC

- CORS 정책 : Cross-Origin Resource Sharing 정책으로, 서로 다른 origin간의 resource sharing을 제한하는 것 (보안의 목적)
- Proxy server : 방화벽 기능 / 웹 필터 기능 / 캐쉬 데이터, 공유 데이터 제공 등의 기능을 제공하는 중간 서버