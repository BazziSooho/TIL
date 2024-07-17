
## 함수 구조 : 
- input(parameter) -> function body -> output f(x)[return value]

## 매개변수와 인자

- 매개변수(parameter) : 함수를 정의할 때, 함수가 받을 값을 나타내는 변수. 보통 def 옆에 있음
- 인자(argument) : 함수를 호출할 때, 실제로 전달되는 값. 함수 정의하고 사용할때 있음

  

## 다양한 인자 종류

- Positional Arguments(위치인자) : 함수 호출 시 인자의 위치에 따라 전달되는 인자. 함수 호출 시 반드시 값을 전달해야 함
- 
- Default Argument values(기본 인자 값) :  함수 정의에서 매개변수에 기본 값을 할당. 인자 전달 없으면 기본값 할당
- 
- Keyword Arguments(키워드 인자) 
	- 매개변수와 인자를 일치시키지 않고, 특정 매개변수에 값을 할당 가능
	- 인자 순서 중요 x. 이름 명시하여 전달
	- 호출 시. 키워드 인자는 위치 인자 뒤에 위치해야함

- Arbitrary Argument Lists(임의의 인자 목록)
	- 정해지지 않은 개수의 인자를 처리하는 인자. 함수 정의 시. 매개변수 앞에 *를 붙여 사용. 여러 개 인자를 tuple처리
	- ex) def cal_sum(*args)

- Arbitrary Keyword Argument Lists(임의의 키워드 인자 목록)
	- 정해지지 않은 개수의 키워드 인자를 처리하는 인자. 함수 정의 시. 매개변수 앞에 **를 붙여 사용 여러 인자를 dict로 묶어 처리
	- ex) def print_info(**kwargs)

- 함수 인자 권장 작성순서 : 위치 -> 기본 -> 가변 -> 가변 키워드

- 절대적이진 않음

  

## 재귀 함수 :
- 함수 내부에서 자기 자신을 호출하는 함수(ex. factorial)
- 특정 알고리즘 식을 표현할 때 변수의 사용이 줄어들며, 코드의 가독성이 높아짐
- 1개 이상의 base case가 존재하고, 수렴하도록 작성
- 재귀함수 사용이유 : 문제의 자연스러운 표현, 코드 간결성, 수학적 문제 해결
- 종료 조건 명확히. 반복이 base case에 수렴하도록

##  내장 함수(Built-in Function) : 
- 파이썬이 기본적으로 제공하는 함수
- 유용한 내장함수
- map :
	- 순회 가능한 데이터구조의 모든 요소에 함수를 적용하고, 그 결과를 map object로 반환
	- ex) result = map(str, numbers)

- split : 문자열을. 하나하나 나누어 list 형태로 변환
- zip : 임의의 iterable을 모아 튜플을 원소로 하는 zip object를 반환

##  함수와 Scope

- 함수는 코드 내부에 local scope를 생성하며, 그 외의 공간인 global scope로 구분
- local에 설정된 변수는 global에서 참조 불가능
- 변수의 수명주기는 변수가 선언되는 위치와 scope에 따라 결정됨(built-in, global, local scope)
- 이름 검색 규칙 : 파이썬의 식별자들은 Local -> Enclosed -> Global -> Built-in 순서대로 이름을 찾음(LEGB Rule)

## Global 키워드 

- 변수의 스코프를 전역 범위로 지정하기 위해 사용. local 안에 있는(함수 안에 있는) 변수를 전역 변수로 바꿔주는 keyword
- Parameter에는 Global 사용불가

  

## Packing & Unpacking

- Packing : 여러 개의 값을 하나의 변수에 묶어서 담는 것
	- 변수에 담긴 값들은 튜플 형태로 묶임
	- *는 남는 요소들을 리스트로 패킹하여 할당

- Unpacking

	- Tuple이나 List 등의 객체의 요소들을 개별 변수에 할당
	- *는 리스트의 요소를 언패킹하여 인자로 전달
	- **는 딕셔너리의 키-값 쌍을 언패킹하여 함수의 키워드 인자로 전달


## Lambda : 
- 간단한 연산이나 함수를 한 줄로 표현할 때 사용
- ex) add = lambda x, y : x + y

  

## 꿀팁

- print와 return은 다른 개념. 혼동하기 쉬우니 유의할것

- 위치 인자는 앞에 있을수밖에 없음. 왜인지 생각해볼것

- 내장 함수의 반대는 외장 함수가 아님! bulit-in function과 Function만 있음
  
- 2차원 리스트에 대해 잘 알아둘 것