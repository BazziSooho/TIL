## 상속
- 기존 클래스의 속성과 메서드를 물려받아 새로운 하위 클래스를 생성하는 것
- 상속이 필요한 이유
	- 코드 재사용
	- 계층 구조 형성 가능
	- 유지보수의 용이성
### 클래스 상속
- 예시)
```
class Person :
	def __init__(self,name) :
		self.name = name
		
class Student(Person) 
#Student 클래스가 Person에 상속
```

## 다중 상속

- 둘 이상의 상위 클래스로부터 여러 행동이나 특징을 상속받는 것.
- 상속받은 모든 클래스의 요소를 활용 가능함
- 중복된 속성이나 메서드가 있는 경우 상속 순서에 의해 결정됨 : 
```
class Baby(Dad, Mom) 
# Baby는 Dad와 Mom을 상속받음
# 속성을 찾는 순서는 Baby -> Dad -> Mom 순서
```
- 파이썬에서는 MRO 알고리즘을 사용하여 클래스를 검색
- MRO : Method Resolution Order : 메서드 결정 순서
- super() : 부모 클래스 객체를 반환하는 내장 함수
