# 5주차 미션: React-Messenger: Refactor!💌

안녕하세요 프론트엔드 유시원입니다!

항상 저희의 적절한 발전 방향을 꼭 맞는 과제를 통해 제시해 주시는 운영진 분들께 감사 인사 드립니다.
타입스크립트.. 항상 리액트와 짝이 되어 사용되는 것을 어깨 너머로 많이 보았고,
유망한 기업들의 채용 공고를 올려다 보면 항상 보이는 기술이었기에 꼭 한번 써보고자 하던 와중에
이번 기회를 통해 사용해 보게 되었습니다.

### 타입스크립트 사용후기
너무나도 자유로운 js문법을 사용하다 자꾸 에러가 나서 숨이 막혔습니다.
알고리즘 문제풀이를 파이썬으로 하다가 C++도 아니고 C언어로 풀게 된 기분이었습니다.
그만큼 제가 자유로운 문법 속에서 위험하게 변수 처리, 상태관리를 하고 있다는 것을 알게 되었습니다.
string이나 number처럼 간단한 type 말고도, React.FormEvent<HTMLFormElement>와 같이 이벤트가 발생할 때 적용할 수 있는 type도 정해져 있다는 사실도 알게 되었습니다.

다만 아쉬운 점은 제 과제의 구조가 Firebase와 온라인으로 통신하여 인터넷 상에서 사용자, 채팅과 관련된 data를 받아오는 구조이다 보니,
local에서 작업할 때 자료형을 string[]과 같은 타입으로 명시를 하거나, uid같은 객체 내부 속성을 불러오려고 시도하는 경우 할당될 수 없는 type이라는 오류가 자주 발생합니다.
그래서 어쩔 수 없이 any타입으로 type을 명시해놓은 부분이 많은 점, 참고 부탁드립니다!

아주 Basic한 수준에서 타입스크립트를 써 보았는데, 현재 수많은 기업들이 쓰고 있다는 점은
큰 프로젝트에서 실제로 얼마나 이 기술이 필요하고, 편한지를 나타내는 증거라는 생각이 들었습니다.
당장의 사이드프로젝트에서는 이 정적 타이핑 방식이 답답하게 느껴지지만,
제 진로를 프론트엔드로 결정하게 된다면 제대로 공부하게 될 날이 올 거라는 생각이 들어요 :)
아래 이미지는 인스타툰 데브경수 작가님의 만화 중 한 컷인데, 이번 과제를 통해 프엔 팀원분들께서도 공감할 수 있게 되었을 것 같습니다 ㅎㅎ
![image](https://user-images.githubusercontent.com/50395394/142468836-533022ab-8d39-4d58-a434-55c4f5532768.png)

### Custom Hooks 사용후기
모르고 볼 때는 너무 어려워 보였는데, 생각보다 구현이 크게 어렵지 않아 기뻤습니다.
제 과제에서 Home 컴포넌트와 ChatList 컴포넌트에서 친구 목록 나열, 검색이 이루어지는데 UI가 많이 중복되는 부분을
useSearch라는 Custom Hook을 사용해 획기적으로 단축할 수 있었습니다.
이 부분 외에 다른 UI 중복이 있나 찾아 보았는데, 딱히 없어서 custom hook은 하나만 쓰게 되었네요!
Custum hook 덕에 코드 가독성 측면에서의 발전을 이룬 것 같아 기쁩니다 :)

### Context API... (구현X)
꼭 써보고 싶습니다. 이번에 적용하지 못한 게 지금에 와서야 내심 아쉽습니다.
좀 더 부지런했다면 할 수도 있었을텐데..... 지금은 다음번을 기약하지만 꼭! 말뿐만이 아니라 진짜 하겠습니다
구현하다 잘 안되면 @codeKiuk 님께서 적용해 놓은 패턴을 보고 공부하곤 하는데.. Star해 두고 공부 자료로 쓰겠습니다 :)