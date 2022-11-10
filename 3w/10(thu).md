## 오늘의 회고 ヾ(•ω•`)o

### 조건에 맞는 리드미를 정리하고 테스트에 맞는 코드 작성하기

<br>

### 느낀 점 😃

클래스를 어떤 기능이나 흐름을 기준으로 분리해야 하는 것부터, 기능 구현을 어떻게 할 지에 대한 고민이 너무 많았다. 그래도 혼자 고민하는 시간이 많은 덕분에 생각보다 코드를 작성하는데는 지난번만큼 오랜 시간이 걸렸던 것 같진 않다.

<br>

### 클래스 💩

🔱 디렉토리 -> view, domain, lotto
<br>

- view: 입출력되는 클래스 모임
  - 입력값을 관리하는 클래스
    - (ex. 로또 구입 금액, 당첨 번호 + 보너스 번호)
  - 출력값을 관리하는 클래스
    - (ex. 로또 구매 개수, 당첨 내역, 수익률 메시지)
  - Profit: enum으로 당첨 수익 계산하는 클래스
  - 입력값을 받아올 때 발생하는 예외를 탐지하는 클래스
- domain: 게임에서 주요 기능을 하는 클래스 모임
  - 생성되는 로또를 관리하는 클래스(로또 한 장)
  - Lotto에서 생성되는 모든 로또들을 관리하는 클래스(전체 로또 n장)
  - 중복되지 않는 랜덤 숫자 6개(로또)를 생성해주는 클래스
- lotto: 전체적인 로또 게임을 진행하는 클래스 모임
  - 로또 게임을 실행하는 클래스
  - 로또가 진행되는 클래스

<br>

어제 오늘 계속 고민하다가, 피드백에서 리드미에는 주요 기능에 관해 작성하는 걸 주로 해야할 것 같아 빼두었다..!

<br>

### 테스트 💩

사실 테스트 기능은

```(java)
assertThat(~).isEqualTo();
assertThatThrownBy(()->~)
```

밖에 안해보았는데, 이번에는
예외처리, 예외 처리 문구까지 일치하는지 확인해주는 AssertJ 친구들이 있어 신기했다..
<br>

처음 테스트를 배웠을 때는 왜 굳이 테스트까지 만들어서 실행하나 싶었는데, 프리코스에서 테스트를 만들면서 굳이 출력을 다 찍어보지 않아도 테스트를 기능 별로 작성하여 문제가 생긴 부분을 바로 찾고, 테스트를 통해 문제를 발견하는 일들을 겪으면서 필요성을 느꼈다.