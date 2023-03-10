# 삼색볼펜법을 통한 스터디 내용 정리


##  - chapter_08

- 스터디 중 삼색볼펜법으로 체크한 부분들을 팀원들과 공유한 내용입니다.
- 빨간색과 파란색은 스터디원끼리 표시했던 공통된 부분을 정리합니다.
- 초록색은 스터디원들끼리 표시했던 개별적인 부분을 정리합니다.

## 🔴 빨강

*	253p. 3번째문단 2번째줄 객체지향 설계의 핵심은 협력을 위해 필요한 의존성은 유지하면서도 변경을 방해하는 의존성은 제거하는데 있다.
*	257p. 3번째문단 3번째줄 의존성이란 의존하고 있는 대상의 변경애 영향을 받을 수 있는 가능성이다.
*	260p. 4번째문단 1번째줄 클래스가 사용될 특정한 문맥에 대해 최소한의 가정만으로 이뤄져 있다면 다른 문맥에서 재사용하기가 더 수월해진다. 이를 컨텍스트 독립성이라고 부른다.
*	261p. 4번째문단 1번째줄 이처럼 컴파일타임 의존성을 실행 컨텍스트에 맞는 적절한 의존성으로 교체하는 것을 의존성 해결이라고 부른다.
*	268p. 1번째문단 1번째줄 추상화란 어떤 양상,세부사항,구조를 좀 더 명확하게 이해하기 위해 특정 절차나 물체를 의도적으로 생략하거나 감춤으로써 복잡도를 극복하는 방법이다.
*	271p. 3번째문단 1번째줄 의존성은 명시적으로 표현돼야 한다.
*	273p. 3번째문단 1번째줄 해결 방법은 인스턴스를 생성하는 로직과 인스턴스를 사용하는 로직을 분리하는 것이다.
*	274p. 2번째문단 1번째줄 사용과 생성의 책임을 분리하고, 의존성을 생성자에 명시적으로 드러내고, 구제 클래스가 아닌 추상클래스에 의존하게 함으로써 설계를 유연하게 만들 수 있다.




## 🔵 파랑

*	254p. 4번째문단 2번째줄 의존성은 방향성을 가지며 항상 단방향이다.
*	258p. 3번째문단 1번째줄 여기서 중요한 것은 런타임 의존성과 컴파일 의존성이 다를 수 있다는 것이다. 사실 유연하고 재사용 가능 한 코드를 설계하기 위해서는 두 종류의 의존성을 서로  다르게 만들어야 한다.
*	260p. 1번째문단 4번째줄 따라서 컴파일타임 구조와 런타임 구조 사이의 거리가 멀면 멀수록 설계가 유연해지고 재사용 가능해진다.	
*	266p. 3번째문단 1번째줄 다른 환경에서 재사용하기 위해 내부 구현을 변경하게 만드는 모든 의존성은 바람직하지 않은 의존성이다.
*	267p. 5번째문단 1번째줄 더 많이 알고 있다는 것은 더 적은 컨텍스트에서 재사용 가능하다는 것을 의미한다.			
*	276p. 2번째문단 2번쨰줄 따라서 변경될 확률이 거의 없는 클래스라면 의존성이 문제가 되지 않는다.		
*	281p. 1번째문단 2번째줄 훌륭한 객체지향 설계란 객체가 어떻게 하는지를 표현하는 것이 아니라 객체들의 조합을 선언적으로 표현함으로서 객체들이 무엇을 하는지를 표현하는 설계다.

## 🟢 초록
*	254p. 3번째문단 1번쨰줄 이처럼 어떤 객체가 예정된 작업을 정상적으로 수행하기 위해 다른 객체를 필요로 하는 것을 두 객체 사이에 의존성이 존재한다고 말한다.
*	257p. 3번째문단 3번째줄 의존성이란 의존하고 있는 대상의 변경에 영향을 받을 수 있는 가능성이다.
*	259p. 4번째문단 3번째줄 유연하고 재사용 가능한 설계를 창조하기 위해서는 동일한 소스코드 구조를 가지고 다양한 실행 구조를 만들 수 있어야 한다.
*	271p. 3번째문단 2번째줄 명시적인 의존성을 사용해야만 퍼블릭 인터페이스를 통해 컴파일타임 의존성을 적절한 런타임 의존성으로 교체할 수 있다.
*	274p. 3번째문단 1번쨰줄 클래스 안에서 객체의 인스턴스를 직접 생성하는 방식이 유용한 경우도 있다. 주로 협력하는 기본 객체를 설정하고 싶은 경우가 여기에 속한다.

