## 내가 생각하는 클래스 ✈

- lotto
  - application
  - lotto (발행된 로또를 저장하는)
  - lottoNumberGenerator (6개의 숫자 생성해 lotto에 넣어주는)
  - answer (model->정답 로또 저장, 관련 정보 처리?하는)
- Game
  - announce
  - lottoGame (model->)
  - controller (게임 진행을 관리하는)
- View
  - input (입력값 관리)
  - output (출력값 관리)
  - valid (입,출력 예외 검출)

<br>

## 기능 부분 🛬

- 조건에 로또 숫자들을 먼저 생성하고 정답 로또들을 입력받기 때문에 아마도 로또 숫자들을 모두 저장하고 나중에 생성된 정답 숫자들과 비교해야할 것 같다.
