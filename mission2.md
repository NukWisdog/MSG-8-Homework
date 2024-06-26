1. 용어
(1) CLI(Command-Line Interface)/GUI(GRAPHIC User Interface)
*CLI : 명령어 인터페이스로, 주로 터미널을 통해 상호작용 하는 방식
*GUI : 입출력 등의 기능을 알기 쉬운 아이콘 등의 그래픽으로 나타난 것

(2) Local/Remote
*Local : 우리가 사용하고 있는 컴퓨터
*Remote : 원격 저장소

(3) Repository(Repo 저장소)
*프로젝트가 존재하는 저장 공간

(4) Branch(브랜치)
*Repository의 공간에서 독립적으로 어떤 작업을 하기 위한 공간

(5) Commit
*소스코드의 업데이트를 확정, 확정된 순간의 코드 상태를 메시지와 함께 Git Ropo에 저장

(6)Pull/Push
*Pull : 원격저장소의 내용을 로컬저장소에 끌어오는 것
*Push : Commit한 내용을 원격 저장소에 업로드

2. 협업

(1) 원격 저장소에 공동작업자 추가하기
*github에 Repository를 만든다.
*Repository에서 Setting->Collaborators에서 팀원 (Github 아이디나 이메일)을 추가 
*팀원에게 초대 매일 전송
*초대 메일을 받은 팀원이 초대를 수락

(2) 작업 환경 구성
*각 작업자의 컴퓨터에 깃과 연결할 폴더를 생성
*공동 작업에서 사용할 이름과 이메일 주소를 지정
 (-global은 빼고)

3. 깃에 첫 번째 푸시

(1) 원격 저장소에 푸시를 한다.
*원격 저장소 주소 복사 후 깃의 origin에 복사한 주소를 지정
*git push 명령으로 origin의 master 브랜치에 커밋을 올린다.
*-u 옵션을 사용하면 다음부터 git push 명령만으로 원격 저장소의 master branch에 commit을 올릴 수 있다.

4. 첫 번째 push가 아니라 pull 먼저

(1) 공동작업자는 대표작업자가 올린 내용을 먼저 pull를 작업
* 원격 저장소는 복제하는 작업으로 최신 커밋을 pull 하지 않으면 push가 이루어지지 않는다.
* 최신 커밋 정보를 가져온 후 지역 저장소의 커밋을 올려야 한다.

5. 브랜치 사용

* 각자 다른 기능을 맡아서 작업할 때 사용
* 각자의 작업이 master 브랜치에 있는 문서들과 섞이지 않도록 새 브랜치를 만들어 버전을 관리
* 각 팀원이 만든 새 브런치 역시 원천 저장소에 그대로 push할 수 있습니다. 각 팀원이 만든 새 브런치 역시 원천 저장소에 그대로 push할 수 있다.

(1) 새로 만든 브랜치 push 하기

* 최신 커밋 가져오기
* 지역저장소에 브랜치 만들고 체크아웃
* 새로운 파일 생성후 테스트

(2) 깃허브 사이트에서 New pull request
(3) pull request 메시지를 작성한 후 Create pull request를 누르면 협업 중인 저장소에 풀 리퀘스트가 전송이 됨
(4) 협업 중인 풀 리퀘스트는 공동 작업자 중 누구나 살펴보고 병합할 수 있다.
