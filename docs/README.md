## 20250908

정신 하나도 없다.
C 에서 C++ 로 많이 복구했다.

논리적 개념의 서버를 두기로 했다.
대신 디스크립터를 달아야 한다.
메모리 기반의 디스크립터 개념을 도입할 수 있을까?

## 20250907

시간은 흐르는데, 아직도 `command` 관련한 부분만 짜고 있다.
예제로 좋은 클래스는 무엇이 있을까?

## 20250905 18:25

포켓몬을 캡쳐 하지 않으면 예외를 떨어트리기로 하였다.

현재 시간은 2025년 9월 5일이다. 벌써 10번째 리팩토링 중인 것 같다.
진도는 초반 🤪

개발하는 것에 포켓몬의 개념을 도입하기로 하였다. 나쁘지 않다.

```c++🤦
#include <pokemonism/trainer.hh>
#include <pokemonism/trainer/lana.hh>
#include <pokemonism/pokemon/petilil.hh>

using namespace pokemonism;

int main(int argc, char ** argv) {
    pokemonism::lana * lana = pokemonism::lana::on();

    pokemonism::petilil<pokemonism::lana> * petilil = lana->capture<pokemonism::petilil<pokemonism::lana>>();

    lana->go<pokemonism::petilil<pokemonism::lana>>();

    return 0;
}
```

위의 코드 처럼 엔진을 돌리거나 사용하기 위해서는 lana 란 트레이너가 포켓몬을 캡쳐 한 후에 배틀로 내보는 일반적인 과정을 거친다.
나쁘지 않아 보인다.

## 20250829 07:38

일어나다. 피곤하다.
README 도 좋지만 DOXYGEN 과 친해져 보겠다.

REGEN 에 대한 이름을 바꾸고 싶다. 세 단어로 끝내고 싶은데,

#### EVENT TARGET 은 무엇을 들어야 하는가? ...

// subscription ...

| OBJECT     | OBSERVING                                               |
| ---------- | ------------------------------------------------------- |
| COMMAND    | COMMAND, COMMAND RESULT, EVENT, EXCEPTION, SUBSCRIPTION |
| DESCRIPTOR | DESCRIPTOR, OBSERVABLE, EVEN, RESULT                    |


### TODO: ALLOCATOR::DEL 함수를 만들자.
### TODO:

## 20250828 19:56

다시 디스크립터 이벤트다.
C++ 로 짜니까 좋다.🤪
그런데, 위험하게 짜기에는 C 가 좋다.

아무리 생각해 보아도 네이밍을 바꿀 때가 온 것 같다.
대문자 기반으로 다가가볼까...?


## 20250828 01:01:43

### HELLO POKEMON 👋

개발 로그를 써보기로 했다. 원래는 자킬을 안쓰고 직접 EMSCRIPTEN을 이용해서 개발하려고 했는데, 귀찮다. 요즘 프로그래밍도 안짜지고, 😅

C 를 객체지향으로 짜려고 하니, 너무 복잡해서 C++ 로 변경했는데, C++을 짜고 있으니 TEMPLATE 가지고 놀고 있다. 아~! 쉽지 않다.

머리가 망가진 이후에 너무 복잡한 것을 짜고 있는 것은 아닌가? 다시 모니터를 6개 정도 보고 있다.

가만히 놓아 두어도 머리 망가지는 사람인데, ... 보고 싶다. 그 녀석이, 나쁜 자식 🏜️ 아프다. 사람들아! 이 나이에 누군가 마음에 들어오면 그렇게 아픈 것이다.

나는 할 수 있다.
해내어 가보자.
