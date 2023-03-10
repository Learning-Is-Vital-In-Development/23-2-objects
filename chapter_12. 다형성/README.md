# 삼색볼펜법을 통한 스터디 내용 정리

### 🔴 빨간색 부분
* 392p 상속의 진정한 목적은 코드 재사용이 아니라 다형성을 위한 서브타입 계층을 구축하는 것이다.
* 392p 이번 장에서는 상속의 일차적인 목적이 코드 재사용이 아닌 서브타입의 구현이라는 사실을 이해하는 것만으로도 충분하다.
* 392p 포함 다형성을 위해 상속을 사용하는 가장 큰 이유는 상속이 클래스들을 계층으로 쌓아 올린 후 상황에 따라 적절한 메서드를 선택할 수 있는 메커니즘을 제공하기 때문이다.
* 393p 객체지향 패러다임의 근간을 이루는 아이디어는 데이터와 행동을 객체라고 불리는 하나의 실행 단위 안으로 통합하는 것이다.
* 399p 이처럼 부모 클래스에서 정의한 메서드와 이름은 동일하지만 시그니처는 다른 메서드를 자식 클래스에 추가하는 것을 메서드 오버로딩이라고 부른다.
* 401p 이처럼 행동 관점에서 상속과 다형성의 기본적인 개념을 이해하기 위해서는 상속 관계로 연결된 클래스 사이의 메서드 탐색 과정을 이해하는 것이 가장 중요하다.
* 405p 부모 클래스(Lecture) 타입으로 선언된 변수에 자식 클래스(GradeLecture)의 인스턴스를 할당하는 것이 가능하다. 이를 업캐스팅이라고 부른다.
* 406p 반대로 부모 클래스의 인스턴스를 자식 클래스 타입으로 변환하기 위해서는 명시적인 타입 캐스팅이 필요한데 이를 다운캐스팅(downcasting)이라고 부른다.
* 407p 이처럼 컴파일타임에 호출할 함수를 결정하는 방식을 정적 바인딩(static binding), 초기 바인딩(early binding), 또는 컴파일타임 바인딩(compile-time binding)이라고 부른다.
* 407p 이처럼 실행될 메서드를 런타임에 결정하는 방식을 동적 바인딩(dynamic binding) 또는 지연 바인딩(late binding)이라고 부른다.
* 408p 객체가 메시지를 수신하면 컴파일러는 `self` 참조라는 임시 변수를 자동으로 생성한 후 메시지를 수신한 객체를 가리키도록 설정한다. 동적 메서드 탐색은 `self`가 가리키는 객체의 클래스에서 시작해서 상속 계층의 역방향으로 이뤄지며 메서드 탐색이 종료되는 순간 `self` 참조는 자동으로 소멸된다.
* 409p 메시지를 수신했을 때 실제로 어떤 메서드를 실행할지를 결정하는 것은 컴파일 시점이 아닌 실행 시점에 이뤄지며, 메서드를 탐색하는 경로는 `self` 참조를 이용해서 결정한다.
* 410p 메시지는 상속 계층을 따라 부모 클래스에게 자동으로 위임된다.
* 413p 자식 클래스가 부모 클래스의 메서드를 오버라이딩하면 자식 클래스에서 부모클래스로 향하는 메서드 탐색 순서 때문에 자식 클래스의 메서드가 부모 클래스의 메서드를 감추게 된다.
* 416p 동일한 코드라고 하더라도 `self` 참조가 가리키는 객체가 무엇인지에 따라 메서드 탐색을 위한 상속 계층의 범위가 동적으로 변한다.
* 419p `self` 전송은 자식 클래스에서 부모 클래스 방향으로 진행되는 동적 메서드 탐색 경로를 다시 `self` 참조가 가리키는 원래의 자식 클래스로 이동시킨다.
* 419p 결과적으로 `self` 전송이 깊은 상속 계층과 계층 중간중간에 함정처럼 숨겨져 있는 메서드 오버라이딩과 만나면 극단적으로 이해하기 어려운 코드가 만들어진다.
* 421p 이해할 수 없는 메시지를 처리할 수 있는 동적 타입 언어는 좀 더 순수한 관점에서 객체지향 패러다임을 구현한다고 볼 수 있다.
* 421p 정적 타입 언어에는 이런 유연성이 부족하지만 좀 더 안정적이다. 모든 메시지는 컴파일타임에 확인되고 이해할 수 없는 메시지는 컴파일 에러로 이어진다.
* 424p `super` 참조의 정확한 의도는 '지금 이 클래스의 부모 클래스에서부터 메서드 탐색을 시작하세요'다.
* 424p 이처럼 `super` 참조를 통해 메시지를 전송하는 것은 마치 부모 클래스의 인스턴스에게 메시지를 전송하는 것처럼 보이기 때문에 이를 super 전송(super send)이라고 부른다.
* 429p 이처럼 자신이 수신한 메시지를 다른 객체에게 동일하게 전달해서 처리를 요청하는 것을 위임(delegation)이라고 부른다.
* 434p 현재 대부분의 객체지향 언어들이 클래스에 기반하고 있기 때문에 다형성을 위해 클래스 기반의 상속이 널리 사용되지만 프로토타입 언어처럼 위임을 통해 객체 수준에서 상속을 구현하는 언어들도 존재한다는 사실을 기억하기 바란다.
* 434p 중요한 것은 클래스 기반의 상속과 객체 기반의 위임 사이에 기본 개념과 메커니즘을 공유한다는 점이다.

### 🔵 파란색 부분
* 391p 강제 다형성은 언어가 지원하는 자동적인 타입 변환이나 사용자가 직접 구현한 타입 변환을 이용해 동일한 연산자를 다양한 타입에 사용할 수 있는 방식을 가리킨다.
* 391p 매개변수 다형성은 제네릭 프로그래밍과 관련이 높은데 클래스의 인스턴스 변수나 메서드의 매개변수 타입을 임의의 타입으로 선언한 후 사용하는 시점에 구체적인 타입으로 지정하는 방식을 가리킨다.
* 397p 부모 클래스와 자식 클래스에 동일한 시그니처를 가진 메서드가 존재할 경우 자식 클래스의 우선순위가 더 높다.
* 398p 이처럼 자식 클래스 안에 상속받은 메서드와 동일한 시그니처의 메서드를 재정의해서 부모 클래스의 구현을 새로운 구현으로 대체하는 것을 메서드 오버라이딩이라고 부른다.

### 🟢 초록색 부분
* 392p 비록 상속 관계를 기준으로 설명을 진행하지만 이번 장에서 다루는 내용은 상속 이외에도 포함 다형성을 구현할 수 있는 다양한 방법에 공통적으로 적용할 수 있는 개념이라는 사실을 기억하기 바란다.
* 434p 중요한 것은 클래스 기반의 상속과 객체 기반의 위임 사이에 기본 개념과 메커니즘을 공유한다는 점이다. 이 사실을 이해하면 다형성과 상속, 나아가 객체지향 언어를 바라보는 여러분의 시각이 달라질 것이다.
