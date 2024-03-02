# Nuxt

## nuxt가 뭐야?

> Vue.js 애플리케이션을 구축하기 위한 프레임워크.

## nuxt 장점

- 검색 엔진 최적화
- 초기 프로젝트 설정 비용 감소와 생산성 향상
- ESLint, Prettier
- 라우터, 스토어 등의 라이브러리 설치 및 설정 파일 필요 X
- 파일 기반의 라우팅 방식, 설정 파일 자동 생성

## nuxt 노트

- pages 폴더안에 넣어둔 대로 자동으로 라우팅이 됨. (`.nuxt/router.js`에서 확인 가능.)
- 동적 라우팅의 경우 파일 앞에다가 꼭 `_id.vue`와 같은 형태로 작성해 주어야 한다.
- console 관련 경고 `'no-console': process.env.NODE_ENV === 'production' ? 'error' : 'off',`를 추가할 것
