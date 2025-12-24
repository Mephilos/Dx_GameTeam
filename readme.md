# C++ Game Framework Project (DxLib)

상용 엔진을 사용하지 않고, C++와 DxLib를 이용하여 게임의 핵심 시스템과 물리 로직을 구현한 팀 프로젝트입니다.

## 작성한 핵심 소스코드 목록
연산의 기반이 되는 **선형대수학 라이브러리**와 **물리 충돌 시스템** 구현을 주로 전담하였습니다.

### 1. 연산 (`scr/math`)
- **[Matrix.cpp](MyGame/scr/math/Matrix.cpp) / [Quaternion.cpp](MyGame/scr/math/Quaternion.cpp)**
  - 4x4 행렬 연산 및 쿼터니언 회전 로직 직접 구현
  - 상용 엔진의 도움 없이 물체의 변환(Transform) 파이프라인 구축

### 2. 물리 및 충돌 (`scr/collision`)
- **[CollisionFunction.cpp](MyGame/scr/collision/CollisionFunction.cpp)**: 선분(Line), 사각형(Rect), 원(Circle), 캡슐(Capsule) 간의 기하학적 충돌 판정 알고리즘 구현한 커스텀 물리 체크 시스템 구축.

### 3. 그래픽스 액터 시스템 (`scr/graphic`, `scr/actor`)
- **[Model.cpp](MyGame/scr/graphic/Model.cpp) / [AnimationDx.cpp](MyGame/scr/graphic/AnimationDx.cpp)**: Dx라이브러리를 사용한 3D 리소스 로딩 및 애니메이션 제어.
- **[ActorManager.cpp](MyGame/scr/actor/ActorManager.cpp)**: 객체 생명 주기 관리 및 게임 오버 상태 판정 로직

---

## 작업 내역
- 프로젝트 진행 당시 작성된 **[개발 백로그](_image/backlog.png)**를 함께 첨부합니다.
- 담당자 'SIM' 항목을 통해 위 소스코드들에 대한 실제 작업 내역을 확인하실 수 있습니다.

