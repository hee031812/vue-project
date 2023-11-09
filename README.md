### vue를 이용한 포트폴리오 사이트 만들기   
Vue.js(뷰)는 웹 애플리케이션을 개발하기 위한 JavaScript 프론트엔드 프레임워크입니다.   
Vue.js는사용자인터페이스(UI)를 만들고 관리하기 위한 기능을 제공하며, 다른 라이브러리나 프레임워크와 통합하기 쉽습니다.     
      
1. 선언적 렌더링: Vue.js는 HTML 템플릿과 JavaScript 코드를 결합하여 UI를 설명할 수 있는 선언적     렌더링을지원합니다. 이것은 개발자가 어떻게 UI가 보이는지 정의하고 데이터 상태에 따라 자동으로   
업데이트되도록 하는데 도움이 됩니다.   
      
2. 컴포넌트 기반 구조: Vue.js는 컴포넌트 기반 아키텍처를 사용하여 UI를 작은 독립적인 부분으로 나눌 수 있습니다. 각 컴포넌트는 자체의 템플릿, 스타일, 및 로직을 가지며, 재사용이 용이합니다.   
      
3. 양방향 데이터 바인딩: Vue.js는 데이터와 UI 간의 양방향 데이터 바인딩을 제공합니다. 데이터의 변경은 자동으로 UI에 반영되고, UI의 변경 역시 데이터에 반영됩니다.   
   
4. 디렉티브: Vue.js에서 디렉티브는 v-로 시작하는 특별한 속성으로, HTML 요소에 특별한 동작을 부여합니다.    예를 들어, v-if, v-for, v-model과 같은 디렉티브를 사용하여 조건부 렌더링, 반복, 양방향 바인딩 등을 처리할 수 있습니다.   
    
5. 라우팅: Vue Router를 사용하여 클라이언트 사이드 라우팅을 구현할 수 있습니다. 이것은 SPA(Single Page Application)를 만들 때 유용합니다.   
      
6. 상태 관리: Vue.js 애플리케이션에서 중앙 상태 관리를 위해 Vuex를 사용할 수 있습니다. 이것은 상태를 관리하고 컴포넌트 간에 데이터를 공유하는 데 도움이 됩니다.   
   
라이프사이클 훅: Vue 컴포넌트는 생성, 갱신, 소멸 등의 라이프사이클 이벤트를 가지며, 이를 사용하여 특정 시점에 코드를 실행할 수 있습니다.
    
     
<span style="color:red">한줄요약<span>   
> Vue.js는 선언적 렌더링, 컴포넌트 기반 구조, 양방향 데이터 바인딩, 디렉티브, 라우팅, 상태 관리,    라이프사이클 훅 등을 제공하는 JavaScript 프론트엔드 프레임워크입니다.   
    

### 설치하기   
1. `npm init vue@latest`   
2. `프로젝트 이름 설정`   
3. √ Project name: ... vue-project   
   √ Add TypeScript? ... <span style="color: blue">No</span> / Yes   
   √ Add JSX Support? ... No / <span style="color: blue">Yes</span>   
   √ Add Vue Router for Single Page Application development? ... No / <span style="color: blue">Yes</span>   
   √ Add Pinia for state management? ... <span style="color: blue">No</span> / Yes   
   √ Add ESLint for code quality? ... No / <span style="color: blue">Yes</span>   
   √ Add Prettier for code formatting? ... No / <span style="color: blue">Yes</span>   
4. `npm install`   
5. `npm run format`   
6. `npm run dev`   
7. gsap 설치: `npm install gsap`
8. sass 설치: `npm install sass`
9. lenis 설치: `npm install @studio-freight/lenis` 
