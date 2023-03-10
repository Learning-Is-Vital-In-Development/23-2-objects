# 삼색볼펜법을 통한 스터디 내용 정리

## Ch_13. 서브클래싱과 서브타이핑

<br>

### 🖍

- 439p. 1번째문단 1번째줄: 객체의 타입을 결정하는 것은 내부의 속성이 아니라 객체가 외부에 제공하는 행동이라는 사실을 기억하라.
- 443p. 2번째문단 1번째줄: 서브타입의 인스턴스는 슈퍼타입의 인스턴스로 간주될 수 있다.
- 445p. 7번째문단 2번째줄: 클라이언트가 두 타입이 동일하게 행동할 것이라고 기대한다면 두 타입을 타입 계층으로 묶을 수 있다.
- 450p. 3번째문단 1번째줄: 인터페이스를 클라이언트의 기대에 따라 분리함으로써 변경에 의해 영향을 제어하는 설계 원칙을 인터페이스 분리 원칙 이라고 한다.
- 457p. 2번째문단 1번쨰줄: 중요한 것은 클라이언트 관점에서 행동이 호환되는지 여부다. 그리고 행동이 호환될 경우에만 자식 클래스가 부모 클래스 대신 사용될 수 있다.
- 458p. 4번째문단 1번째줄: 행동 호환성과 리스코프 치환 원칙에서 한 가지만 기억해야 한단면 이것을 기억하라. 대체 가능성을 겨정하느 것은 클라이언트다.

<br>

### 🖌

- 435p. 5번째문단 3번째줄: 타입 사이의 관계를 고려하지 않은 채 단순히 코드를 재사용하기 위해 상속을 사용해서는 안된다.
- 444p. 1번째문단 2번째줄: 클라이언트의 관점에서 두 클래스에 대해 기대하는 행동이 다르다면 비록 그것이 어휘적으로 is-a 관계로 표현할 수 있다고 하더라도 상속을 사용해서는 안된다.
- 459p. 2번째문단 1번째줄: 결론적으로 상속이 서브타이핑을 위해 사용될 경우에만 is-a 관계다.

<br>

### 🪛

- 437p. 2번째문단 4번째줄: 일반적으로 instaceof처럼 객체의 타입을 확인하는 코드는 새로운 타입을 추가할 때마다 코드 수정을 요구하기 때문에 개방-폐쇄 원칙을 위반한다.
