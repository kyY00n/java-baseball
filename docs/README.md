# 기능 목록

## 절차

- [x] 게임을 시작할 수 있다
- [x] 게임이 완전히 종료될 때까지 반복할 수 있다

## 객체가 할 수 있는 일

### 컴퓨터 (Game, 상대방)

- [x] 게임의 진행상태를 관리할 수 있다. (시작, 일시정지, 종료)
- [x] 게임을 시작(초기화)할 수 있다.
    - [x]  숫자 정하기: 랜덤으로 숫자를 정할 수 있다.
    - [x] `camp.nextstep.edu.missionutils.Randoms`의 `pickNumberInRange()` 을 사용한다.
- [x]  게임을 종료할 수 있다.

### GameScanner (사용자 입력 처리 모듈)

- [x]  사용자 입력을 받아 전달할 수 있다.
    - 키보드로 입력받은 숫자로 `Number` 객체를 생성한다.
- [x]  3스트라이크 시 게임 진행 여부를 입력 받을 수 있다.

### GamePrinter (게임 문구 출력 모듈)
- [x] 게임 시작 문구를 출력할 수 있다.
- [x] 게임 결과를 출력할 수 있다.

### GameResultCalculator (결과 계산 모듈)
- [x]  스트라이크/볼/낫싱 여부를 계산한다.
    - [x] 스트라이크 개수 계산
    - [x] 볼 개수 계산
- [x] 3스트라이크 여부를 계산할 수 있다.


### 숫자 (Number)
- [x]  숫자의 자릿수를 따로 관리할 수 있다.
- [x]  세자릿수를 받아 자릿수를 분리할 수 있다.
- [x]  숫자를 입력했을 때 값을 검증할 수 있다.
    - [x] 올바르지 않을 경우 `IllegalArgumentException` 예외를 던진다.
    - [x] 이 예외를 받은 프로그램은 종료된다.


### 게임 종료 후 명령 (FinishInput)

- [x] 숫자를 인자로 받아 의미를 가진 객체를 반환할 수 있다.
- [ ] 올바르지 않은 인자의 경우 `IllegalArgumentException` 예외를 발생할 수 있다. 
