# CSR & SSR

> Client와 Server 어느 쪽에서 렌더링을 할꺼니?

## 간단하게

CSR은 Client 즉 브라우저에서 렌더링을 처리하는 방식. 쉽게 말하면 데이터 수정이 발생하면 브라우저가 스스로 DOM을 수정함.

SSR은 브라우저가 변경이 필요할 때마다 서버에 요청을 해서 수정하는 방식임.

## 서론

렌더링 방식은 화면에 HTML을 그려내는 것을 누가 할까에 따라서 나뉘게 된다.

보통 JS 기반의 웹 프레임워크들(React, Vue 등)은 `index.html`을 컨테이너 역할을 할 DOM Element를 필요로 한다. 그 컨테이너는 보통 다음과 같은 모습이다.

```html
<html>
  <head>
    <title>Title</title>
  </head>
  <body>
    <div id="app"></div>
  </body>
</html>
```

프레임워크에서 Application instance를 만들게 되면

---

환경설정 및 에셋이 모두 불러와 진 뒤 `.mount` 매서드가 호출되면
