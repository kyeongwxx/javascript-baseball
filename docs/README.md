# 구현 기능 목록

## [✅] 기능 1 - 게임 시작 문구를 출력하는 함수 구현

게임 시작 시 "숫자 야구 게임을 시작합니다." 문자열 출력

- 출력 값은 [MissionUtils 라이브러리]에서 제공하는 `Console.print()` 메서드를 사용

## [✅] 기능 2 - 서로 다른 임의의 수 선택 함수 구현

컴퓨터는 1에서 9까지 서로 다른 임의의 수 3개를 선택

- 임의의 수는 [MissionUtils 라이브러리]에서 제공하는 `Random.pickNumberInRange()` 메서드를 사용

## [✅] 기능 3 - 숫자 입력 문구 출력 및 사용자 입력 값을 받는 함수 구현

"숫자를 입력해주세요 : " 문자열 출력 및 사용자 입력 값을 입력받음

- 출력 및 입력은 [MissionUtils 라이브러리]에서 제공하는 `Console.readLine()` 메서드를 사용

## [✅] 기능 4 - 사용자의 입력 값(3자리 수)의 유효성 검사 함수 구현

사용자가 입력한 값이 유효한지 확인하고 잘못된 값을 입력한 경우 `throw`문을 사용해 예외를 발생시킨후 애플리케이션 종료

- 3자리의 숫자
- 1에서 9까지의 숫자 (0 제외)
- 서로 다른 숫자
- 입력 값은 [MissionUtils 라이브러리]에서 제공하는 `Console.readLine()` 메서드를 사용

## [✅] 기능 5 - 사용자의 입력 값(3자리 수)을 판별하는 함수 구현

사용자가 입력한 값과 컴퓨터가 생성한 임의의 수를 비교하여 사용자 입력 값에 따른 결과를 반환

- 예) 컴퓨터가 생성한 임의의 수가 425일 때
  - 123 입력 시 1스트라이크 / 같은 수가 같은 자리에 있을 경우 스트라이크
  - 456 입력 시 1볼 1스트라이크 / 같은 수가 다른 자리에 있을 경우 볼
  - 789 입력 시 낫싱 / 같은 수가 전혀 없을 경우 낫싱

## [✅] 기능 6 - 게임 종료 문구를 출력하는 함수 구현

게임 종료 시 "3개의 숫자를 모두 맞히셨습니다! 게임 종료 게임을 새로 시작하려면 1, 종료하려면 2를 입력하세요." 문자열 출력

- 기능 5에서 반환된 결과를 판별하여 3스트라이크일 경우 게임 종료 문구 출력
- 그 외의 경우 기능 3으로 이동하여 임의의 수를 모두 맞출 때까지 반복
- 출력 값은 [MissionUtils 라이브러리]에서 제공하는 `Console.readLine()` 메서드를 사용

## [✅] 기능 7 - 사용자의 입력 값(재시작/종료)의 유효성 검사 함수 구현

사용자가 입력한 값이 유효한지 확인하고 잘못된 값을 입력한 경우 `throw`문을 사용해 예외를 발생시킨후 애플리케이션 종료

- 숫자 1 또는 2

## [✅] 기능 8 - 사용자의 입력 값(재시작/종료)을 판별하는 함수 구현

사용자가 입력한 값에 따른 결과를 반환

- 1 입력 시 새로운 임의의 수 생성 후 기능 2로 이동
- 2 입력 시 애플리케이션 종료
  - 애플리케이션 종료는 [MissionUtils 라이브러리]에서 제공하는 `Console.close()` 메서드를 사용
