Redux
==

보통 React랑 많이 쓰이는 상태관리 도구이다. 
vue나 여러가지에서도 쓰일 수 있지만 vue나 angular는 자체적으로 상태관리를 가지고 있기 때문에 React에서 쓰인다.(React가 라이브러리라고 정의한 이유와 동일하다.)

[그림]

* action을 만들지 않고 initial.compA = 'b' 바로 이렇게 할 수 없다는 것이 단점이지만 안전성, 코드를 추적함으로 실수를 방지할 수 있다.

#### action
action을 만들 때 최대한 이름 짓는 것을 피하자
* 액션(객체)를 함수로 만들어주자
* 액션을 정말 함수로 만들어버리는 것이 아니고 return 해주는 부분을 계속해서 객체(액션)을 만들 수 있게 만들자는 말이다.

#### reducer
리듀서를 생성하는 이유는 위에서 말했듯이 만약 initial.compA = 'b'로 덮어버린다면 그 전 코드를 알 수 가 없기 때문이다. 우리가 만들어준 action을 받아 매번 새로운 state를 생기게 하고 그 전 객체를 대체해주는 역할이다. 불변성!!
+ default 구문을 만들어주는 이유는 대표적으로 action type에 오타가 났을 경우 그것을 방지해 주기 위함이다.
---
[redux 공식 문서](https://redux.js.org/)

[redux 해석](https://deminoth.github.io/redux/)


