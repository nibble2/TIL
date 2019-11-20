Hash 함수
==

#### 해시 함수는 문자열을 받아서 숫자를 반환하는 함수


+ 일관성이 존재해야 한다.
    - 만약 'apple'을 넣었을 때 '4'를 반환한다면 어떠한 상황에서도 계속 'apple'을 넣었얼 '4'를 반환해야 한다.

    - 다른 단어가 들어가면 다른 숫자가 나와야 한다.

#### 해시 테이블을 사용하는 예
1. 해시 테이블로 조회하기
2. 중복된 항목을 방지하기

~~~
voted = {}
def check_voter(name):
  if voted.get(name):
    print("kick them out!")
  else:
    voted[name] = True
    print("let them vote!")

check_voter("tom")
check_voter("mike")
check_voter("mike")
~~~