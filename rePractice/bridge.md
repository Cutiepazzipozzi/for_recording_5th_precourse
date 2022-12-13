## 내가 생각하는 클래스 ✈

- View
  - InputView (입력값 받아오는 + 예외 사항 처리)
  - OutputView (다리 그림? 및 결과 메시지 출력)
  - Valid (Input값의 예외 처리를 위한)
- Bridge (모델?)
  - BridgeGame ()
  - BridgeMaker (정답 다리를 생성하는)
  - BridgeRandomNumberGenerator (다리 숫자 랜덤 생성 로직), BridgeNumberGenerator (인터페이스)
- BridgeGame (컨트롤러?)
  - GameController (게임을 진행하는)

## 좀 고민해봐야 할 것

- BridgeGame을 어떻게 활용해 정답 값과 입력 값을 비교하고 경우에 따라 게임을 진행할 지!

BridgeGame - 정답을 가져 인자로 받아오는 입력값과 비교

\*\*
