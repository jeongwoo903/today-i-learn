# Vue

## Vue 왜 쓸까?

- vue는 프레임워크임. 라이브러리가 아님.
- vue는 react와 같이 wep-app을 만들때 씀
- SSR를 가능하게 함.
- react보다 쉬움.
- 스타일 통일이 좋음. 개발자마다 코드 스타일이 비슷해 대규모 코드 관리에 좋음.
- HTML 렌더링이 빠름. 근데 거의 ms단위로..
- 표준 HTML을 템플릿으로 확장하여 사용.

## 공식문서 톺아보기

### Vue란?

> 사용자 인터페이스를 구축하기 위한 JavaScript 프레임워크입니다. 표준 HTML, CSS 및 JavaScript를 기반으로 구축되며, 단순한 것 부터 복잡한 것 까지 사용자 인터페이스를 효율적으로 개발할 수 있는 컴포넌트 기반 프로그래밍 모델을 제공

### 핵심기능 2가지

1. 선언적 렌더링
   > 표준 HTML을 템플릿으로 확장하여, JS 상태를 기반으로 HTML을 선언적으로 작성할 수 있다.
2. 반응성
   > JS 상태를 추적하고 자동으로 DOM을 업데이트 해줌.

### Vue의 프레임워크 특성 (프로그래시브 프레임워크)

Vue는 프레임워크여서 자유로운 개발이 한정되어 있을 수도 있다고 생각했다.  
하지만 Vue는 프로젝트의 형태나 크기에 따라 점진적으로 설계할 수 있게 해 두었다.

### 싱글 파일 컴포넌트 (SFC)

컴포넌트의 논리(JavaScript), 템플릿(HTML) 및 스타일(CSS)을 하나의 파일에 캡슐화함.

### Vue-CLI 사용하려면

`npm install -g @vue/cli`

하지만 다응과 같은 방법으로도 vue의 기능을 사용할 수 있다.
`<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>`

### vue-nuxt 프로젝트 생성

`npm init nunxt-app [project name]`