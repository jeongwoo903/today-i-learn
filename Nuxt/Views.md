# Nuxt

## Views

## app.vue

- Root Component인 파일.
- pages 디렉토리에 있는 모든 페이지 컴포넌트의 공통으로 사용되는 레이아웃을 정의.
- 전역적으로 사용되는 CSS 파일이나 플러그인들을 설정할때 사용.
- 어플리케이션 전역에서 사용되는 상태 관리 라이브러리를 설정.

## Components

- 재사용가능한 Asset들을 Component 폴더에 넣음.

## Pages

- pages/directory/index.vue 형식으로, 디렉토리 이름에 따라 자동 라우팅을 해줌.

## Layouts

- Header와 Footer 같은 공통적으로 사용되는 부분에 대한 Vue 파일이다.
- 기본적으로 고정할 레이아웃은 `default.vue`로 특정 레이아웃을 사용하기 위해선 다음과 같은 문법을 사용하면 된다.

```ts
definePageMeta({
  layout: "edit-layout",
});
```
