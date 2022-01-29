# 원티드 프리온보딩 프론트엔드 코스 사전과제

## 공통. MouseCircle

### 구현 방법

mousedown, mousemove, mouseup 이벤트리스너를 추가하여 마우스 클릭시 커서 주위에 원이 나타나는 효과를 주었습니다.

### 구현 이유

공통 기능이므로 컴포넌트를 만들어서 App에 추가하는 방식으로 하면 중복되는 코드를 줄이고 간단하게 공통 모듈로 사용할 수 있기에 컴포넌트를 추가하는 방식으로 구현하였습니다.

### 실행 방법

어플리케이션 실행 후 DOM 안에서 어느 곳을 클릭하던지 해당 기능을 사용하실 수 있습니다.
<img width="80%" src="https://user-images.githubusercontent.com/36434219/151656821-c5542afa-2834-4b95-be39-6a77603848bc.gif">
<br>

## 2. Toggle

### 구현 방법

checked라는 state를 만들어서 mouseup라는 이벤트 발생시마다
state를 업데이트시켜서 해당 컴포넌트를 리렌더링시키고 그때 css 효과를 주게끔 구현하였습니다.

Props로 defaultChecked, color, disabled을 추가하여 옵션으로 적용할 수 있도록 하였습니다.

### 구현 이유

ON / OFF의 대명사인 Toggle을 라이브러리 없이 구현하는 경험을 해보고 싶었고 자세히 보면 색이 채워질 때 동시에 채워지는 것이 아니라 방향성을 가지고 채워지므로 그런 디테일을 구현해보고 싶었습니다.

### 에러 로그

색깔을 방향성 있게 채우고 비우게 하는 것에서 난관이 있었습니다.
그래서 css 속성을 검색하여 background 속성 중 linear-gradient라는 속성이 이 경우에 제격이라는 것을 알아내어 적용시켰습니다.

### 실행 방법

토글 스위치에 마우스를 갖다대고 길게 클릭하시거나 짧게 클릭하시면 스위치가 토글됩니다.
<img width="80%" src="https://user-images.githubusercontent.com/36434219/151656859-6dd95f4a-162c-481a-9e1a-fdd2a8017597.gif">
