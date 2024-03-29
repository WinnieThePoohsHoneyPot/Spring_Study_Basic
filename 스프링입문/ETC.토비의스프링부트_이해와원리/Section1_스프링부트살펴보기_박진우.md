# CH00. Prolog : 스프링 부트 살펴보기

------------

## [SpringBoot]
### "스프링 부트(Spring Boot)란?"
> 스프링 부트(Spring Boot)는 스프링을 기반으로 실무 환경에 사용 가능한 수준의 독립실행형 애플리케이션을 복잡한 고민 없이 빠르게 작성할 수 있게 도와주는 여러가지 도구의 모음이다.

### "스프링 부트의 핵심 목표"
- 매우 빠르고 광범위한 영역의 스프 개발 경험을 제공
- 강한 주장을 가지고 즉시 적용 가능한 기술 조합을 제공하면서, 필요에 따라 원하는 방식으로 손쉽게 변형 가능
- 프로젝트에서 필요로 하는 다양한 비기능적인 기술(내장형 서버, 보안, 메트릭, 상태 체크, 외부 설정 방식 등) 제공
- 코드 생성이나 XML 설정을 필요로 하지 않음

------------

## [Containerless]
### "Serverless"
> 서버에 대한 설치 및 관리를 개발자가 신경쓰지 않아도 서버 애플리케이션을 개발, 배포, 운영하는 것이 가능

### "Containerless"
> 서블릿 컨테이너를 설치, 관리를 하기위해 개발자가 들이는 수고와 시간을 제거

### "Containerless의 적용"
- 서블릿 컨테이너의 동작(.xml)들이 스프링 부트에 의해 제공
- 개발자는 이를 신경쓰지 않고, 일단 개발을 시작하고 서버를 띄우고 실행시킬 수 있음.
- 스프링 부트를 사용하여 메인 메소드를 실행시키면 Servlet Container와 Spring Container가 함께 실행됨
    - **“Stand Alone Application”: 독립 실행형 애플리케이션**

------------

## [Opinionated]
### “스프링 프레임워크의 설계 철학”
- 극단적인 유연함 추구
- 다양한 관점을 수용
- Not opinionated
- 수많은 선택지를 모두 포용
- 하지만, 이러한 **선택에 대한 고민을 개발자들이 직접 해야함.**
    - 꽤 많은 시간을 들여 어떤 기술을 어떻게 사용해야할지 고민

### “스프링 부트의 설계 철학”
- **“Opinionated”**
- 일단 정해주는 대로 빠르게 개발하고 고민은 나중에
- 스프링을 잘 활용하는 뛰어난 방법을 제공

### “사용 기술과 의존 라이브러리 결정”
- 업계에서 검증된 스프링 생태계 프로젝트, 표준 자바 기술, 오픈소스 기술의 종류와 의존관계, 사용 버전 등을 정해줌
- 각 기술을 스프링에 적용하는 방식(DI 구성)과 디폴트 설정값 제공

### “유연한 확장”
- 스프링 부트에 내장된 디폴트 구성을 커스터마이징 하는 매우 자연스럽고 유연한 방법 제공
- 스프링 부트가 스프링을 사용하는 방식을 이해한다면, 언제라도 스프링 부트를 제거하고 원하는 방식으로 재구성 가능
- 스프링 부트처럼 기술과 구성을 간편하게 제공하는 나만의 모듈 작성

------------

## [스프링 부트의 이해]
### “스프링 부트를 이용한 개발 방법”
- 부트가 결정한 기술과 구성, 디폴트 설정을 수용
- 외부 설정 파일을 이용한 설정 변경 방법을 활용
- 아주 빠르게 개발을 시작할 수 있음

### “스프링 부트를 이용한 개발의 오해와 한계”
- 애플리케이션 기능 코드만 잘 작성되면 된다.
- 스프링을 몰라도 개발을 잘할 수 있다.
- 스프링 부트가 직접적으로 보여주지 않는 것은 몰라도 된다.
- 뭔가 기술적인 필요가 생기면 검색을 해서 해결한다.

### “스프링 부트를 이해하게 되면”
- 스프링 부트가 스프링의 기술을 어떻게 활용하는지 배우고 응용할 수 있다.
- 스프링 부트가 선택한 기술, 자동으로 만들어주는 구성, 디폴트 설정이 어떤 것인지 확인할 수 있다.
- 필요할 때 부트의 기본 구성을 수정하거나, 확장할 수 있다.
- 나만의 스프링 부트 모듈을 만들어 활용할 수 있다.