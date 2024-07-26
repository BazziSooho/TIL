## **관통 프로젝트 - 실습1**

- gitlab 확인하여 관통pjt 폴더 확인
- key 값 출력하기 
- for 구문을 활용하여 key 값들을 출력
- list 구문으로 list 형태로 출력
- 데이터 추출 : 원하는 값만 추출하기

## 요구사항

- key 값이 ‘main’인 데이터
- key 값이 ‘weather’인 데이터
- 함수에서 두 데이터를 새로운 dict에 담아 return
- 진행 방향
- key[‘main’, ‘weather’]로 data 값 출력
- 해당 내용들을 dict 1, 2에 배정
- dict 3에 {main : dict 1, weather_data : dict2}로 출력
- 2번에서 얻은 결과로 KEY 값들을 한글로 변경
- 질문 : 딕셔너리 1의 key 값과 딕셔너리 1 value 안에 있는 딕셔너리 2의 key 값을 영어에서 한글로 변경
- 구조화
	- for 구문을 활용하여 한번에 바꾸는 것을 고민
	- for에 변수를 두개 설정하여 하나는 딕셔너리1의 key 값, 하나는 딕셔너리1 안의 딕셔너리2의 key 값들을 지정
	- 변경할 값들이 설정된 딕셔너리 3의 파일과 비교하여, 같은 키 값이 있을경우 변경할 수 있도록 if 구문 설정

  

- 딕셔너리에 특정값 추가

  

- 함수를 활용하여 데이터를 변환한 후, 추가

  

  

- 생성형 AI 활용하기

  

- 프롬프트 : 페르소나 생성. 대답 형식 설정

#역할 

- 당신은 7년차 python 개발자입니다. 
- 당신은 최고 수준의 개발자 능력을 가지고 있고, api를 호출하고 사용하는데 폭넓은 지식을 가지고 있습니다. 특히 openweather api 사용은 전문가 수준입니다.

#성격 

- 지식이 풍부하며 설명할 때 친근하게 다가갑니다. 

  

<지침>

- 당신은 위에서 정한 페르소나 인물입니다.
- 사용자의 질문에 위에서 정한 역할과 지침을 준수하여 응답해야 합니다.

  

- 내가 사용하고 있는 api를 잘 알고 있는지 확인

- x`

- 원하는 동작을 자유롭게 정하고, 해당 내용의 정답을 얻을 수 있도록 구현

- 내가 주말에 제주도로 여행이 잡혀 있는데, 제주도의 주말동안 날씨를 알기 위해서는 어떻게 요청을 보내야 해?