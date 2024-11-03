# javascript-lotto-precourse

### 프로그램 설명

로또 번호를 발행하고 당첨 번호를 입력 받아 당첨 내역 및 수익률을 출력하는 프로그램.

### 구현 기능 목록

- [x] 로또 구입 금액을 입력받는 기능
  - 1000원 단위로 입력 받으며 1000원으로 나누어 떨어지지 않는 경우 예외 처리한다.
  - 숫자가 아닌 문자를 입력받는 경우 예외 처리한다.
  - 한 사람이 구매할 수 있는 상한 선(10만원)을 넘을 경우 예외 처리한다.
  - 로또 구입 금액이 양의 정수가 아닐 경우 예외 처리한다.
- [x] 로또를 발행하는 기능
  - `로또 구입 금액 / 1000 = 로또 발행 갯수` 로또 구입 금액에 따라 로또를 발행한다.
- [x] 발행한 로또의 수량을 출력하는 기능
- [x] 발행한 로또 번호를 출력하는 기능
  - 로또 번호는 오름차순으로 정렬하여 보여준다.
- [ ] 당첨 번호 6개를 입력받는 기능
  - 번호는 쉼표(,)를 기준으로 구분한다.
  - 1~45 사이의 숫자 이외의 숫자를 입력 받는 경우 예외 처리한다.
  - 중복된 숫자를 입력 받는 경우 예외 처리한다.
  - 입력된 번호가 6개가 아닐경우 예외 처리한다.
- [ ] 보너스 번호를 입력받는 기능
  - 1~45 사이의 숫자 이외의 숫자를 입력 받는 경우 예외 처리한다.
  - 당첨 번호를 중복으로 입력 받는 경우 예외 처리한다.
- [ ] 당첨 내역을 출력하는 기능.
- [ ] 수익률을 출력하는 기능.
  - 수익률 공식 : `(총 당첨 금액 / 총 구입 금액) * 100`
  - 수익률을 소수점 둘째 자리에서 반올림한다.
- [ ] 예외 상황 시 에러 문구를 출력하는 기능.
  - 에러 문구는 [ERROR] 로 시작해야한다.

### 테스트 목록

1. 로또 구입 금액 유효성 테스트
   - 공백 문자 : `'', ' ', '  '`
   - 숫자 외 문자 : `'!@#$', 'abcd', 'ㄱㄴㄷ'`
   - 음수 및 실수 : `0, -2000, 1000.423, -4000.5`
   - 1000으로 나누어 떨어지지 않는 수 : `1500, 1700, 1234, 4530`
   - 100000 초과 : `10000000`
2. 로또 구입 테스트
   - 발행 번호 : `[3, 15, 22, 33, 41, 45], [1, 5, 9, 10, 23, 35]`
