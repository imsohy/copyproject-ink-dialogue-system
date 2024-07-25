# copyproject-ink-dialogue-system
## 프로젝트 개요
ShapedByRainStudios의 Youtube 재생목록 'Unity2D + INK Dialogue System'을 카피해 써보고, 써본 소스코드들을 저장하기 위한 곳입니다..
2.choices-implemented 부터 카피해보았습니다.소스코드의 몇 부분에 코드와 동영상을 함꼐 보면서 이해한 바가 주석으로 추가되어있습니다.

* 유투브 재생목록 : [Unity2D + INK Dialogue System](https://www.youtube.com/playlist?list=PL3viUl9h9k78KsDxXoAzgQ1yRjhm7p8kl, "youtube playlist로")
* 원 프로젝트 Github : [shapedbyrainstudios/ink-dialogue-system](https://github.com/shapedbyrainstudios/ink-dialogue-system, "github link로")

원 깃헙에 있는 코드를 그대로 새 유니티 프로젝트로 가져올 수 있습니다.
## 업로드 노트
### 2024-07-24
create branch 2-choices-implemented
#### 내용: 
NPC와 기본적인 대화시스템 구축
onclick() No Function 문제 : [Button Onclick() No Function 문제](https://mingxoxo-record.tistory.com/23)
#### 후기:
전 분명히 전부 해결했다고 생각했는데, 컴포넌트에 오브젝트를 연결하는 부분에서 Script가 아닌 GameObject를 연결해야하더군요...스크립트를 연결하는것과 게임오브젝트를 연결하는 것과
표시가 동일하게 될 때가 있어서 조심해야겠습니다.
중점적으로 살펴봤던 건 일단 *싱글톤 클래스 프로그래밍*이었던 것 같습니다. 클래스에 static instance를 생성하고, 다른 클래스에서 클래스의 인스턴스를 받아서 쓸 때는 해당 클래스의 인스턴스를 받아서 쓰는
프로그래밍이라니...*알고리즘*공부도 제껴두고 있는데. 노마드코더에서 나오는 *프로그래밍 기법*에 대해서 진작에 공부라도 좀 해뒀어야 되었던걸까요. 재미있는 기법들이 상당히 많네요.
그 이외에 *Coroutine*에 대한 사용 방법또한 있었습니다.
기본적으로 다이얼로그 UI를 숨기고, 띄우고, JSON 다이얼로그 파일을 가져오고. 선택지를 처리하는 과정에 대한 메서드를 작성하는 방법을 볼 수 있었던 것 같습니다.
