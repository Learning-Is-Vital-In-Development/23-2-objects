# 삼색볼펜법을 통한 스터디 내용 정리
		
		
		
		
		


# Object 부록 A. 계약에 의한 설계 

### 🔴 빨간색 부분

* 538p 1번째문단 1번째줄 여기서 눈여겨볼 부분은 한쪽의 의무가 반대쪽의 권리가 된다는 것이다. 
* 538p 6번째문단 1번쨰줄 계약에 의한 설계를 이용하면 오퍼레이션의 시그니처를 구성하는 다양한 요소들을 이용해 협력에 참여하는 객체들이 지켜야 하는 계약 조건을 명시할 수 있다.
* 541p 1번째문단 1번째줄 일반적으로 사전 조건은 메서드에 전달된 인자의 정합성을 체크하기 위해 사용된다.
* 545p 1번째문단 1번째줄 사전조건과 사후 조건은 각 메서드마다 달라지는 데 반해 불변식은 인스턴스 생명주기 전반에 걸쳐 지켜져야 하는 규칙을 명세한다.
* 546p 3번째문단 1번째줄 첫 번째 규칙은 협력에 참여하는 객체에 대한 기대를표현하는 계약 규칙이고 두번째 규칙은 교체 가능한 타입과 관련된 가변성 규칙이다. 
* 547p 3번째문단 2번째줄 계약에 의한 설계는 협력을 올바르게 설계하기 위해 고려해야 하는 설계 원칙이고 설계 방법이지 특정한 수현 메커니즘이 아니다.
* 555p 일찍 실패하기 마지막 문장 차라리 문제가 발생한 그 위치에서 프로그램이 실패하도록 만들어라. 문제의 원인을 파악할 수 있는 가장 빠른 방법은 문제가 발생하자마자 프로그램이 일찍 실패하게 만드는 것이다.
* 561p. 파란글씨 서프타입의 리턴 타입은 공변성을 가져야 한다.
* 567p. 파란글씨 서브타입의 메서드 파라미터는 반공변성을 가져야 한다.
* 572p. 1번째문단 1번째줄 진정한 서브타이핑 관계를 만들고 싶다면 서브타입에 더 강력한 사전조건이나 더 완화된 사후조건을 정의해서는 안 되며 슈퍼타입의 불변식을 유지하기 위해 항상 노력해야 한다.
* 547p. 3번째문단 2번째줄 계약에 의한 설계는 협력을 올바르게 설계하기 위해 고려해야 하는 설계 원칙고 설계 방법이지 특정한 수현 메커니즘이 아니다.
* 547p 5번째문단 2번째줄 계약에 의한 설계는 협력을 올바르게 설계 하기 위해 고려해야 하는 설계 원칙과 설계 방법이지 특정한 구현 메커니즘이 아니다.
* 555p [일찍 실패하기(Fail Fast)] 마지막 문단 마지막 문장 문제의 원인을 파악할 수 있는 가장 	빠른 방법은 문제가 발생하자마자 프로그램이 일찍 실패하게 만드는 것이다.
* 565p 4번째문단 1번째줄 이처럼 부모 클래스에서 구현된 메서드를 자식 클래스에서 오버라이딩할 때 부모 클래스에서 선언한 반환타입의 서브타입으로 지정할 수 있는 특성을 리턴 타입 공변성 이라고 부른다. 





### 🔵 파란색 부분

* 538p  (02 계약에 의한 설계 아래) 파란 점 1번째문단 1번째줄 협력에 참여하는 각 객체는 계약으로부터 이익을 기대하고 이익을 얻기 위해 의무를 이행한다.
* 538p  (02 계약에 의한 설계 아래) 파란 점 2번째문단 1번째줄 협력에 참여하는 각 객체의 이익과 의무는 객체의 인터페이스 상에 문서화된다.
* 545p (불변식의 두 가지 특성) 파란 점 1번째문단 1번째줄 불변식은 클래스의 모든 인스턴스가 생성된 후에 만족돼야 한다. 이것은 클래스에 정의된 모든 생성자는 불변식을 준수해야 한다는 것을 의미한다. 
### 🟢 초록색 부분


