## axios
- 뷰에서 권고하는 **HTTP 통신 라이브러리**
- `Promise` 기반의 HTTP 통신 라이브러리
  - promise : 자바스크립트의 비동기 처리 패턴
- 상대적으로 다른 HTTP 통신 라이브러리에 비해 문서화가 되어 있고, API가 다양함
- https://github.com/axios/axios
- 가장 많이 쓰는 라이브러리

### ajax
- 비동기적 웹 어플리케이션 제작에 사용
- 일반적으로 많이 사용 `jQuery.ajax`

### vue-resource
- github, vue의 이전 공식 라이브러리
- 최근 관리가 되지 않음

### 자바 스크립트의 비동기 처리 패턴
- `callback`
- `promise`
  - https://joshua1988.github.io/web-development/javascript/promise-for-beginners/
- `promise + generator`
- `async & await`
- [자바 스크립트 비동기 처리와 콜백 함수](https://joshua1988.github.io/web-development/javascript/javascript-asynchronous-operation/)
- [자바스크립트 Promise](https://joshua1988.github.io/web-development/javascript/promise-for-beginners/)


### axios github
- 예시
- 주요 메서드
- Custom instance default
- Error Handling
- Canceling
- Interceptor

### Promise의 세가지 상태
- `new Promise()`로 프로미스를 생성하고 종료할 때, 3가지 상태를 가짐
  - Pending : 비동기 로직 처리 전
  - Fulfilled : 비동기 처리 완료 및 promise가 결과 값 반환
    ```javascript
    new Promise(function(resolve, reject) {
      resolve(); // resolve 실행시, 이행 상태로 변환
      reject(); // 실패 상태
    });
    ```
    - 이행 상태 이후, `.then(...)` 함수등으로 연접 가능
  - Rejected : 비동기 처리 실패 혹은 오류 발생
    ```javascript
    getDate().then().catch(...) // 이와 같이 구성 가능
    ```