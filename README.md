# java-racingcar-precourse

## 2주차 우테코 프리코스

### 구현 기능 목록

#### 메인

##### 뷰
- [x] 사용자는 쉼표를 기준으로 구분하여 5자 이하로 경주할 자동차에 이름을 부여할 수 있다. 
- [x] 시용자는 몇 번의 이동을 할 것인지 숫자로 입력할 수 있다.
- [x] 사용자가 잘못된 값을 입력할 경우, `IllegalArgumentException`을 발생시킨 후 애플리케이션은 종료한다.

##### 자동차
- [ ] 전진 혹은 멈출 수 있다.

##### 자동차 경주 게임
- [ ] 입력받은 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
- [ ] 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다.
- [ ] 우승자는 한 명 이상일 수 있다. 쉼표를 이용하여 구분한다.

---

### 기능 요구 사항

초간단 자동차 경주 게임을 구현한다.

- 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
- 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
- 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
- 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
- 전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
- 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
- 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
- 사용자가 잘못된 값을 입력할 경우 `IllegalArgumentException`을 발생시킨 후 애플리케이션은 종료되어야 한다.

---

### 프로그래밍 요구 사항

- indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.
    - 예를 들어 while문 안에 if문이 있으면 들여쓰기는 2이다.
    - 힌트: indent(인덴트, 들여쓰기) depth를 줄이는 좋은 방법은 함수(또는 메서드)를 분리하면 된다.
- 3항 연산자를 쓰지 않는다.
- 함수(또는 메서드)가 한 가지 일만 하도록 최대한 작게 만들어라.
- JUnit 5와 AssertJ를 이용하여 정리한 기능 목록이 정상적으로 작동하는지 테스트 코드로 확인한다.
    - 테스트 도구 사용법이 익숙하지 않다면 아래 문서를 참고하여 학습한 후 테스트를 구현한다.
        - [JUnit 5 User Guide](https://junit.org/junit5/docs/current/user-guide)
        - [AssertJ User Guide](https://assertj.github.io/doc)
        - [AssertJ Exception Assertions](https://assertj.github.io/doc)
        - [Guide to JUnit 5 Parameterized Tests](https://assertj.github.io/doc)

---

### 라이브러리

- `camp.nextstep.edu.missionutils`에서 제공하는 `Randoms` 및 `Console` API를 사용하여 구현해야 한다.
- Random 값 추출은 `camp.nextstep.edu.missionutils.Randoms`의 `pickNumberInRange()`를 활용한다.
- 사용자가 입력하는 값은 `camp.nextstep.edu.missionutils.Console`의 `readLine()`을 활용한다.   
   
   
#### 사용 예시

0에서 9까지의 정수 중 한 개의 정수 반환
```
Randoms.pickNumberInRange(0, 9);
```