# NextJS_Study
## 기존 SPA의 단점
페이지를 불러올 때 필요한 모든 자바스크립트 파일을 한번에 불러오는데, 이는 페이지 이동시 이미 파일을 받아왔기 때문에 UI변화가 빠르고, 필요한 데이터는 서버에서 빠르게 
받아올 수 있는것이 장점이다. 이 부분은 SPA의 단점이 되기도 하는데, 한번에 모든 자바스크립트 파일을 불러오기 때문에 리소스가 무거울 경우 시간이 다소 걸리기도 한다. 그리고
검색엔진 최적화인 SEO에 좋지 않은 모습을 보이는데, 이는 클라이언트에서 렌더링을 하기 때문에 검색엔진이 HTML파일이 텅 비어있는것을 보고 컨텐츠를 파악하지 못하는 것이다.

SPA와 서버 사이드 렌더링의 단점을 상쇄하기 위해서 Next.js를 사용하는 것이다.

## 특징
### 1. 사전 렌더링 및 서버 사이드 렌더링
기본적으로 빌드시에 모든 페이지를 렌더링하고 HTML을 가져오기 때문에 사용자에게 빠르게 보여지고 SEO에도 도움이 된다.

### 2. 타입스크립트 내장
웹팩과 바벨을 베이직으로 사용하고 있기 때문에 빠르게 개발을 시작할 수 있고, 타입스크립트 설정을 따로 할 필요 없이 바로 사용 가능하다.

### 3. 간단한 라우팅기능
기존 리액트에서는 라우팅을 위해 react-router 라이브러리 등을 통해 라우팅 설정을 했어야 했는데, 파일 시스템을 기반으로 라우팅이 가능하여 구축이 빠르다.

## getServerSideProps
