## Data Type

  - Numeric Type : int(정수), Float(실수), complex(복소수)
	- 진수 표현 : 0b(2진수), 0o(8진수), 0x(16진수)

- Sentence Sequence type : str(문자열)

- Sequence types : 여러 개의 값들을 **순서대로** 나열하여 저장하는 자료형
	- list : 순서, 중복 있음. 변경 가능. 대괄호로 표기.
		- tuple : 순서, 중복 있음. 변경 불가능. 소괄호로 표기
	- range : 연속된 정수 시퀀스 생성. 변경 불가능. range(시작 값, 끝 값, 증가 값)

- non-sequence type
	- dict : key와 value로 이루어짐. 순서, 중복 없음. 변경 가능. 중괄호로 표현. 
	- set : 순서. 중복 없음. 변경 가능. 중괄호로 표기. 집합자료형이라고도 표현
- 기타 : Boolean, None, Function.
- Collection : 여러 개의 항목 또는 요소를 담는 자료 구조 (str, list, tuple, dict, set)

## Type Conversion(형변환) : 
- 데이터 타입을 다른 데이터 타입으로 변환하는 과정. 암시적, 명시적 

- 암시적 형변환 : 파이썬이 자동으로 수행하는 형변환
- 명시적 형변환 : 프로그래머가 직접 지정해 수행하는 형변환

## 단축평가 : 
- 논리 연산에서 두 번째 피연산자를 평가하지 않고 결과를 결정하는 동작 (아직이해못함)

## 기타 참고사항

- 프로그램의 대부분에서 True는 1, False는 0으로 바라볼 수 있음
- is 는 참조하고 있는 객체 주소가 같은지를 확인. ==는 값만을 확인