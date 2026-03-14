## Autonomous Agent
1. 개요: 뇌(추론)와 몸(행동)의 관계
추론 모델과 Autonomous Agent는 각각 인간의 두뇌와 신체에 비유할 수 있습니다.

추론 모델 (Brain): 복잡한 문제를 해결하기 위한 사고의 흐름을 구성하고 전략을 수립합니다.

Autonomous Agent (Body): 수립된 계획을 바탕으로 실제 외부 도구를 사용해 목표를 달성합니다.

2. Autonomous Agent의 구성 요소
자율 에이전트는 크게 4가지 핵심 모듈로 구성됩니다.

Memory (기억): * Agentic Memory: 추론 과정과 결과를 저장하며, 이는 **장기 기억(Long-term memory)**의 범주에 속합니다.

Planning (계획): 목표를 세부 작업(Sub-tasks)으로 분해하고 실행 순서를 결정합니다.

Action (행동): 결정된 계획을 실제로 수행합니다.

Tools (도구): 검색, API 호출, DB 조회, 문서 생성 등 외부 환경과 상호작용하는 수단입니다.

내일 공부할 영역

### MLOps와 백테스팅 (Backtesting)
성공적인 퀀트 시스템 구축을 위해서는 견고한 인프라가 필수적입니다.

Backtesting: 과거 데이터를 이용해 전략을 시뮬레이션 (생존 편향, 전방 참조 편향 주의).

Walk-forward Analysis: 데이터를 시기별로 나누어 학습과 검증을 반복하며 모델의 강건성(Robustness) 확인.

Deployment: AWS 등 클라우드 환경에서 실시간 데이터 파이프라인과 트레이딩 API(예: LS증권 API) 연결.
