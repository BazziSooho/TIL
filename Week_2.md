# git
## git이란?
- 분산 버전 관리 시스템
- git의 역할 : 코드의 버전을 관리, 개발되어 온 과정 파악, 이전 버전과의 변경 사항 비교
- git의 영역 : WD(working directory), SA(Staging Area), Repository로 구성
- WD : 실제 작업 중인 파일들이 위치하는 영역
- SA : WD에서 변경된 파일 중 다음 버전에 포함시킬 파일들을 선택적으로 추가하거나 제외할 수 있는 중간 준비 영역
- Repository : 버전 이력과 파일들이 영구적으로 저장되는 영역. 모든 버전과 변경 이력이 기록됨.
- commit : sa에서 Repository로 옮기는 행위. snapshot이라고도 부름
## git 기타
- git init : 로컬 저장소 설정(초기화)
- git 로컬 저장소 내엑 또다른 git 로컬 저장소를 만들지 말 것
- 바로 직전 생성한 commit 수정하기 : commit 메시지 수정, commit 전체 수정
- git commit —amend 를 통해 가능. 명령어 사용시 vi 에디터 켜짐
- 버전관리 측면에서 봤을 때, 불필요한 commit을 생성하지 않고, 직전 commit을 수정할 수 있기 때문에 git에서 꼭 필요한 기능
## git을 활용한 원격 저장
- 원격 저장(remote 방식, github, gitlab 등)
- github : copilot 사용 가능(pro 사용시), 개인 기업 둘다 사용하나 개인 위주
- gitlab : 기업이 주로 사용, github는 보안 이슈(copilot ai 데이터 크롤링) 때문.
- git remote add origin remote_repo_url : 로컬 저장소에 원격 저장소 추가
- github -> local repository : pull(업데이트 이미 로컬에 있음) or clone(없다가 새로 다운로드)
- local -> github repository : push
- git의 remote 개념은 클라우드와 개념이 다름. 제한 용량이 작음.
- 원격 저장소에는 commit만 올라감
