# Challenge - Project Management Tool Using Design Pattern

- 6개의 핵심 기능과 세부 기능으로 이루어져 있습니다
- 기능은 참고용으로 원하는 대로 수정을 해도 추가를 해도 좋습니다
- 23가지의 디자인 패턴을 모두 사용해 봅시다
- 디자인 패턴을 사용 할 때와 사용하지 않을 때의 차이를 docs/README.md에 작성해 주세요
- 결과는 화면을 직접 구현해도 콘솔에 출력을 해도 Postman과 같은 툴을 활용해 API 테스트만 해도 좋습니다
- Commit은 세부 작업마다 자주 올려 주세요
- 핵심 기능 구현 시마다 PR을 보냅니다. 다른 사람 PR에 리뷰를 남겨주세요

  ## 프로젝트 설명

  `프로젝트 관리 협업 툴`

  - 디자인 패턴을 활용하여 프로젝트 관리 협업 툴을 만들어 봅시다
  - 이번 과제에서는 디자인 패턴 사용 전/후 차이에 집중해 봅시다
  - 프레임워크, 외부 API 없이 Java만을 이용하여 구현해 봅시다

### Feature 1. 환경 설정  

#### 세부 기능  
 - 애플리케이션 시작에 필요한 설정 들을 AppConfig에서 관리해 보세요  
 - 개발 환경 별(로컬, 배포) 다른 설정이 적용 되도록 해보세요  

#### 디자인 패턴 : Singleton, Factory Method  

### Feature 2. 사용자 관리 기능  
  
#### 세부 기능  
 - 회원가입
 - 로그인/로그아웃
 - 정보 수정

사용자는 이름, 이메일, 권한(관리자, 사용자)의 정보를 가지고 있어요

#### 디자인 패턴 : Builder, Prototype, Abstract Factory  

### Feature 3. 프로젝트 관리 기능  

#### 세부 기능  
 - 프로젝트 생성 : 새 프로젝트 생성 및 초기 설정
 - 프로젝트 구조화 : 업무 단위로 프로젝트를 분류
 - 프로젝트 할당 : 사용자에게 업무를 할당 
 - 프로젝트 상태 관리 : 시작 전, 진행중, 완료 상태 관리

프로젝트는 이름, 업무, 담당자, 중요도, 긴급도, 진행도의 정보를 가지고 있어요

#### 디자인 패턴 : Composite, Decorator, Iterator

### Feature 4. 알림 및 이벤트 시스템

#### 세부 기능  
 - 업무 상태 변경 시 알림이 전송됩니다(우선순위 순서로 전송)
 - 알림은 푸시 알림, 이메일 두 종류가 있어요

#### 디자인 패턴 : Observer, Strategy, Chain of Responsibility, Meditator, Bridge

### Feature 5. 업무 워크플로우 관리

#### 세부 기능  
- 업무 상태 관리: 업무의 진행 중, 검토 중, 완료 상태 관리
- 승인 프로세스: 업무 완료 요청 승인/거절
- 업무 이력 관리: 업무의 변경 사항 추적, 되돌리기

#### 디자인 패턴 : State, Template Method, Command, Memento

### Feature 6. 외부 API 활용

#### 세부 기능  
- 외부 협업 도구 연동: 예를 들어 Slack, Google Calendar 등의 외부 API 통합.
- 데이터 동기화: 외부 시스템에서 가져온 데이터를 애플리케이션 내부 데이터로 변환.
- API 인터페이스 구현: 외부 시스템과 상호작용하는 API 작성

#### 디자인 패턴 : Adapter, Facade, Proxy