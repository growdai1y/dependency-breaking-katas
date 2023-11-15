# 의존성 해체 연습

레거시 코드에서 의존성을 해체하고 이를 테스트할 수 있는 상태로 만드는 연습문제들

## 목표

우리에게는 일부 레거시 코드가 있습니다. 
변경이 필요합니다. 
변경을 하려면 먼저 테스트를 도입해야 합니다. 
테스트를 가능케 하려면 일부 코드를 수정해야 할 수 있습니다. 
우리는 테스트를 도입하기 위해 'Seams'이라 불리는 것을 도입해야 합니다. 
('Seams'은 코드의 변경 없이 동작을 제어하거나 테스트를 삽입할 수 있는 지점을 가리킵니다. 더 자세한 내용은 [래거시 코드 활용 전략](https://www.yes24.com/Product/Goods/64586851) 참고)

테스트 없이 코드를 변경하는 것은 위험하기 때문에 우리는

* 코드를 가능한 적게 변경해야 합니다.
* 가능한 한 자동 리팩토링 도구에 의존합니다.
* 클래스의 공개 API를 변경하면 안 됩니다.

### 의존성 해체 테크닉 대한 과제

* Parametrise Constructor (생성자 매개변수화)
* Subclass And Override Method (서브클래 및 메서드 오버라이드)
* Extract And Override Call (호출 추출 및 오버라이드)
* Replace Global Reference With Getter (글로벌 참조를 Getter로 교체)
* Extract And Override Factory Method (팩토리 메소드 추출 및 오버라이드)

계획된

* Extract Interface (인터페이스 추출)
* Adapt Parameter (매개변수 적응)

### 작업

각 작업은 특정 클래스와 몇몇 협력자를 제시합니다.

* 이 클래스를 테스트 범위에 포함합니다. 핵심 로직의 모든 경로를 커버하는 것을 확인합니다.
* 기존의 테스트 클래스가 첫 번째 테스트 케이스를 가지고 있으며 작동할 수도 있고 아닐 수도 있습니다.
* 협력자를 변경할 수 없습니다. 다른 팀에서도 사용하고 있기 때문입니다.

### 라이센스

[New BSD License](http://opensource.org/licenses/bsd-license.php), 리포지토리의 license.txt 참조.
