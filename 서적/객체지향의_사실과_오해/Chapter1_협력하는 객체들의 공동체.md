# Chap01 협력하는 객체들의 공동체
> 시너지를 생각하라. 전체는 부분의 합보다 크다.

대부분의 사람들은 객체지향에 대해 실세계를 직접적이고, 직관적으로  
모델링할 수 있는 패러다임으로 알고 있다.  

하지만 객체지향의 목표는 실세계를 모방하는 것이 아닌 **새로운 세계를 창조하는 것**이다.  
그 때문에 소프트웨어 개발자 역시 단순하게 실세계를 소프트웨어 안으로 옮겨담는 것이 아니라  
고객과 사용자를 만족시킬 수 있는 **신세계를 창조하는 것**이 그들의 역할이다.

그럼에도 객체지향이 **실세계의 모방**이라는 개념이 계속해서 쓰이는 이유는  
실세계에 대한 비유가 객체지향의 다양한 측면을 이해하고 학습하는 데 유용하기 때문이다.

---

## 협력하는 사람들

### ☕ 커피 공화국의 아침
손님, 캐시어, 바리스타는 서로 **암묵적인 협력 관계**이다.  
따뜻한 커피와 함께 소박한 아침 시간의 여유를 누릴 수 있는 이유는  
각각의 역할과 책임을 다하기 때문이다.

**역할(Role), 책임(Responsibility), 협력(Collaboration)** 은  
우리가 삶을 영위하기 위해 모든 곳에 존재한다.  
소프트웨어 개발 프로젝트 역시 **역할, 책임, 협력**이 존재한다.

### 🧩 역할, 책임, 협력

####  기능을 구현하기 위해 협력하는 객체들
위에서 설명한 실세계의 커피를 주문하는 과정을 그대로 **객체지향**이라는 문맥으로 옮길 수 있다.  
이처럼 객체 지향의 근본 개념은 실세계에서 사람들이 타인과 관계를 맺으며 협력하는 과정과 유사하다.

---

### 🧱 역할과 책임을 수행하며 협력하는 객체들
아리스토텔레스의 말처럼 인간은 타인과 관계를 맺으며 성장하고 발전한다.  
협력의 핵심은 특정한 책임을 수행하는 역할들 간의 연쇄적인 요청과 응답으로 목표를 달성한다는 것이다.  
이런 인간의 세계와 객체의 세계는 유사하다.  

사용자가 마주하는 모든 완성된 시스템의 기능은 객체들이 </br>
성실히 연쇄적인 요청과 응답을 통해 서로 협력해서 일궈낸 결실이다.

객체지향 설계라는 예술은 적절한 객체에게 적절한 책임을 할당하는 것에서 시작된다.  
책임은 객체지향 설계의 품질을 결정하는 가장 중요한 요소다.  

**책임이 불분명한 객체는 애플리케이션의 미래 역시 불분명하게 만든다.**

---

##  협력 속에 사는 객체

객체지향을 객체지향이라고 부르는 이유는 이 패러다임의 중심에 바로 객체가 있기 때문이다.  
객체는 애플리케이션의 기능을 구현하기 위해 존재한다.  
얼마나 협력을 조화롭게 이루는지 결정하는 주체 또한 객체이다.  
즉, 협력의 품질 = 객체의 품질이다.

**객체지향 사고방식**에서 객체는 다음 두 가지 덕목을 갖춰야 한다고 말한다.

1. 객체는 충분히 **협력적**이어야 한다.
    - 외부의 도움을 무시한 채 모든 것을 스스로 처리하고자 하는 전지전능한 객체는 자멸할 것이다.

2. 객체는 충분히 **자율적**이어야 한다.
    - 객체 스스로 결정과 판단에 따라 행동하는 자율적인 존재여야 한다.

---

### 🧊 상태와 행동을 함께 지닌 자율적인 객체

객체는 자신에게 필요한 행동과 상태를 함께 지니고 있어야 한다.  
또한, 다른 객체에 대해 **무엇을 수행하는지**는 알 수 있지만 **어떻게 수행하는지**는 알 수 없어야 한다.  

객체의 관점에서 자율성이란 자신의 상태를 직접 관리하고,  
자신의 상태를 기반으로 스스로 판단하고 행동할 수 있음을 의미한다.

---

### 🤝 협력과 메세지

풍부한 매커니즘을 이용해서 요청하고 응답하는 인간들의 세계와 달리,  
객체지향의 세계에서는 한 가지 의사소통 수단만이 존재한다.  
바로 **메세지**이다.

한 객체는 다른 객체에게 메세지를 전송(요청)하고,  
다른 객체는 그 메세지를 수신(응답)한다.

---

### 🛠️ 메서드의 자율성

객체가 수신된 메세지를 처리하는 방법을 **메서드**라 부른다.  
객체지향 프로그래밍에서는 어떤 객체에게 메세지를 전송하면,  
결과적으로 메세지에 대응되는 특정 메서드가 실행된다.

외부의 요청이 무엇인지를 표현하는 **메세지**와  
요청을 처리하기 위한 구체적인 방법인 **메서드**를 분리하는 것이  
객체의 자율성을 높이는 핵심 매커니즘이며, 이는 **캡슐화** 개념과도 연결된다.

---

### 🧠 객체지향의 본질

> 객체를 지향하라

객체지향 선구자들의 초기 의도와 달리, 대부분의 사람들은 객체지향을 **클래스를 지향하는 것**으로 생각했다.  
객체지향의 중심에 있어야 할 객체로부터 멀어져 간 것이다.  

클래스는 객체지향 프로그래밍 언어에서 매우 중요한 구성 요소인 건 맞지만,  
지나치게 클래스에 집중하면 객체의 **캡슐화**를 저해하고, 클래스를 강하게 결합시키게 된다.

훌륭한 객체지향 설계자가 되기 위해서는
어떤 클래스가 필요한가가 아니라,  
**어떤 객체들이 어떤 메세지를 주고받으며 협력하는가**에 집중해야 한다.

## 🎯 1장의 핵심
> 객체의 역할, 책임, 협력에 집중하라.  
> 객체지향은 객체를 지향하는 것이지, 클래스를 지향하는 것이 아니다.

