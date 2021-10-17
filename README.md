### 새로운 파일 생성
202030430_최선아 라는 폴더를 만들고<BR>
VS로 열어둔다

### 리액트앱 생성
터미널에 아래 코드 입력후 실행<BR>
npx create-react-app 파일명

### 리액트앱 설치가 완료되면
  OPEN Folder>> 만들어둔 리액트앱 <b>안에</b> 들어가서 열기 버튼 누른다
### 지울 코드
  package.json의 17번,18번째 줄을 지운다(16번째줄 쉼표도 지움)
### 리액트앱 실행해보고 종료
  npm start 혹은 localhost:3000
### workspace에서 삭제할 파일
  ```
  APP.css
  APP.test.js
  index.css
  logo.svg(지워봤더니 오류남)
  serviceWorker.js
  setupTest.js
  pakage-lock.json
  ```
### index.js에서 <App />, 주의해가며 삭제할거 삭제하기
  삭제목록
  ```
  import './index.css';<BR>
  import * as serviceWorker from './serviceWorker';
  <React.StrictMode></React.StrictMode>
  밑에 주석들
  ```
### App.js 파일 일부 코드 삭제 
  ```
  import React from 'react';
  import logo ...
  import './app.css...
  <header ...<div>까지 삭제
  ```
  ```
  최종 코드<BR>
  function App(){
  return (<div calssName="App" />)
  }
  export default App;
  ```
  
## 컴포넌트의 기본 형식
```
function App() {
  return (
    <div>Hello React</div>
  );
}

export default App
```

index.js 에서 컴포넌트를 어떻게 사용할까?
```
import ReactDOM from 'react-dom';
import App from './App';

ReactDOM.render(<App />,document.getElementById('root')); 
```
  
+ ReactDOM.render() 함수는 첫번째 인자로 오는 컴포넌트를 그려질 결과로 만들어줍니다
+ 두번째 인자로 오는 것은 그려질 위치로 지정합니다
<br>
+ document.getElementById('root') 함수는 html에서 id가 root인 태그를 지정합니다
+ <App /> 표시를 컴포넌트로 인식합니다
    
