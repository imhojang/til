## Categories



- [Backend Development](#backend-development)
- [Data Structure](#data-structure)
- [Frontend Development](#frontend-Development)
- [JavaScript](#javascript)
- [React.js](#reactjs)
- [Software Development](#software-development)
- [Sorting Algorithm](#sorting-algorithm)
- [Web Foundation](#web-foundation)



### Backend Development

- 노드란?
  - 브라우저 외에도 자바스크립트를 실행할 수 있는 환경.

- 익스프레스란?
  - 노드에서 서버환경을 구축할 때 쓰는 라이브러리

---

### Data Structure

- 빅오란?
  - 알고리즘의 효율성을 나타내는 표기법
  - 알고리즘이 처리해야하는 자료의 크키가 성장함에 따라 알고리즘의 효율이 어떻게 변화하는지 대략적으로 추정할수 있게 도와주는 함수

- 스택이란?
  - LIFO
  - Access On
  - Search On
  - Delete O1
  - Insert O1

- 큐란?
  - Access On
  - Search On
  - Delete O1
  - Insert O1
  - FIFO

- 연결리스트란?
  - 하나의 데이터가 들어가있는 노드를 연결한 선형 자료구조

- 이진탐색트리란?
  - 모두 O log n

- 해시맵이란?
  - 키와 값이 1:1로 매칭되어 저장되어있는 연관배열구조.
  - 키 값 해시함수 해시 그리고 버켓으로 구성되어있다

---

### Frontend Development

- spa란? 장단점은? +
  - 서버로부터 정적 리소스를 초기 요청에 한번만 받고, 이후에 사용자와의 인터렉션에 따라 필요한 데이터만 서버로부터 받아서 기존 페이지의 내부를 수정하는 것.
  - 장점은 네이티브 앱과 유사한 부드러운 사용자 경험, 서버의 과부하가 적다,
  - 단점은 검색엔진 최적화가 되어있지 않다.  비즈니스 로직이 클라이언트에 있으면 보안에 취약. **초기로딩이 느리다**, IE8 지원 X

- SSR이란? 장단점은? +
  - 웹브라우저에서 다른 페이지로 이동할 때마다 서버로부터 정적리소스를 매번 받아 렌더링하는것.
  - 장점은 검색엔진 최적화에 용이.
  - 단점은 서버과부하, **리로딩시 페이지 깜빡임**
- 웹팩이란? +
  - http 프로토콜이 비효율적이기 때문에, 요청 수를 줄이기 위해 웹페이지의 수많은 구성요소 (html css javascript, img, json) 등등을 한번에 받을 수 있도록 번들링 해주는 번들러. 
  - 크로스 브라우징대응
  - 압축

- 바벨이란? +
  - ES 6 를 ES 5 로 전환 해줌 

---

### Javascript

- 스코프란?
  - 함수나 변수를 참조할 수 있는 범위

- 스코프체인이란? +
  - 자바스크립트에서 중첩된 함수에서 전역 스코프까지 상위의 스코프를 차례대로 검색하는 기능.

- 호이스팅이란? +
  - 자바스크립트에서 변수나 함수가 스코프의 상단으로 끌어올려지는 것 처럼 동작하는 특성

- 클로져란? +
  - 내부함수를 반환하는 중첩함수에서 외부함수의 생명주기가 끝나도 **스코프체인을 통해** 외부함수의 스코프를 참조할 수 있는 특성.

- 프로토타입이란? +
  - 모든 자바스크립트 객체는 던더프로토 속성을 통해 자신의 부모역할을 하는 객체에 접근 할 수있고 이 객체를 프로토타입이라고 합니다
  - 객체가 특정한 프로퍼티나 메소드를 해당 객체에서 찾을 수 없을 때, 프로토타입에 접근하여 프로토타입에 들어있는 메소드나 프로퍼티를 위임받아 사용할 수 있습니다.

- 프로토타입 체인이란? +
  - 객체가 특정한 프로퍼티나 메소드를 접근하려 할 때 해당 객체에 없다면 객체가 가진 던더프로토 속성을 따라 자신의 프로토타입이 가진 메소드나 프로퍼티를 검색하는 기능입니다.

---

### React.js

왜 리액트를 쓰나요?

- 편안한 개발경험
  - 직접 dom에 레퍼런스를 잡아서 로직을 만들며 페이지를 만들어도 되지만 귀찮은 DOM 조작과 상태관리를 없애고 오직 기능 개발과 UI 구현에 집중할 수 있도록 도와주기 때문
- 컴포넌트
  - 컴포넌트 별로 나누어서 코드 재사용이 용이함.
  - 컴포넌트 별로 나누어서 프로그램의 복잡성을 낮춤.
- 리액트가 굳이 더 빠른 건 아니다
  - 리덕스를 만들고 리액트 개발에 참여한 댄아브라모브에 의하면 리액트는 바닐라로 만든 페이지보다 더 빠른 것은 아니고 충분히 빠르다고 했다. 
  - 굳이 프레임워크나 라이브러리를 쓸 필요는 없다 하지만 프로젝트 규모가 커짐에 따라 다앙햔 인터페이스와 인터렉션을 제공함에 따라 DOM 요소를 직접 관리하고 코드를 짜는 것은 번거로운 일이기 때문이다.
  - 리액트는 '충분히 빠르다' 라고 표현하는 것이 적절하다.

- 버츄얼돔이 무엇이고 왜 쓰나요?
  - 버츄얼 돔은 리액트에서 상태 변화가 있을 시에 최소한의 렌더링을 만들어주는 역할을 함.

- 왜 리덕스를 쓰나요? 장단점은?

---

### Software Development

- 디자인 패턴이란? +
  - 특정한 상황에서 구조적인 문제해결하기 위해 과거의 개발자들이 설계 노하우에 이름을 붙이고 재이용하기 좋은 형태로 묶어서 정리한 것 디자인패턴.
  - 싱글턴 패턴 - 유일무이한 객체가 필요할 떄 쓰임  예: 관리자@
  - 모듈 패턴- 비공개 변수를 만들 떄 쓰임 @

- TDD란?
  - 테스트 주도 개발이라는 뜻으로서, 테스트를 우선 적고 코드를 적어 나가며 개발을 진행하는 방식

- HOF란?
  - 고차함수. 함수를 일급객체로하는 프로그래밍언어에서 함수를 인자로 받거나 반환하는 함수를 고차함수라고한다.

---

### Sorting Algorithm

- bubble sort
  - best On
  - average O n^2
  - Worst O n^2

- insertion sort
  - best On
  - average O n^2
  - Worst O n^2

- merge sort
  - Best O n log n
  - Average O n log n
  - worst O n log n

- quick sort
  - Best O n log n
  - Average O n log n
  - Worst O n^2

---

### Web Foundation

- 크로스 브라우징이란?
  - 웹 표준 기술을 이용하여 여러 다른 웹기종이나 플랫폼에 구현한 기술이 공통적으로 적용되도록 **웹페이지를 제작하는 것을 말합니다**

- cors란?
  - 브라우저에서 외부 도메인 서버와 통신하는 방식을 표준화한 스펙. 서버와 클라이언트가 정해진 해더를 통해 클라이언트의 요청에 반응하거나 응답할지 결정하는 방식

- cors 해결 방법은?
  - jsonp, proxy server, access control allow origin header 설정, 

- 쿠키란? +
  - 클라이언트 브라우저에 저장되는 키와 값으로 이루어진 작은 파일. 이름, 값, 경로, 그리고 만료날짜 등의 정보가 들어있음. 
  - 쿠키를 사용하는 이유는 http 프로토콜의 특성 때문.
    - connectionless 비연결 지향 - 클라이언트가 요청을 보내면 서버는 그에 맞는 응답을 보내고 연결이 끊어짐
    - **stateless 상태정보유지 안함 - 연결을 끊는 순간 클라이언트와 서버는 통신이 끊어지며 상태정보가 유지되지 않는다.**
  - 서버는 들어오는 요청에 대해 어느 클라이언트인지 판별할 수 있도록, 혹은 상태 정보를 유지할 수 있도록 쿠키를 주고 받는다.
  - **장점: 쿠키에 정보가 있기 때문에 서버로 요청 시 속도가 빠름.**
  - 예: 장바구니, 자동로그인, 오늘은 더이상 이창을 보지 않음

- 세션이란? +
  - **일정시간동안 같은 브라우저로 부터 들어오는 일련의 요구를 하나의 상태로 보고 그 상태를 유지하는 기술. 즉 웹 브라우저를 통해 웹 서버에 접속한 이후로 브라우저를 종료할 때까지 유지되는 상태.**
  - 클라이언트에서 서버로 요청을 보내면 서버는 세션을 만들고 세션 아이디를 클라이언트에게 세션아이디가 담긴 쿠키를 만들라고 합니다.
  - 이 세션 아이디를 통해 클라이언트에 대한 상태 값을 유지합니다.
  - 장점은 사용자에 대한 정보가 서버 쪽에 있기 때문에 보안이 더 나음
  - 단점은 세션은 서버의 자원을 이용하기 때문에 사용자 숫자가 많아지면 생성해야하는 세션의 숫자도 늘어나고, 서버의 메모리가 감당할 수 없게 되고 속도가 느려질수 있다.
  - **정보가 서버에 있기 때문에 처리 속도가 느림**

- 쿠키와 세션의 차이
  - 라이프 사이클
    - **쿠키는 만료시간이 정해져 있고 파일로 저장되어 브라우저를 종료해도 계속해서 정보가 남아있음**
    - 세션도 만료시간이 있지만 브라우저를 종료하는 순간 만료시간에 관계없이 사라짐
  - 저장 위치
    - 사용자 정보파일을 브라우저에 저장하는 쿠키와 달리 세션은 서버 측에서 관리

- 토큰이란?

---

## 탐색

- Binary Search
  - O log n