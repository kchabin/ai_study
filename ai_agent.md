![참고: AI Agents, 비즈니스 워크플로우와의 통합
(1) AI 에이전트의 발전과 시장 트렌드 - Samsung SDS](https://www.samsungsds.com/kr/insights/integrating-ai-assistants-into-business-workflows-part1.html)

## AI Agent
> 인공 지능 에이전트는 환경과 상호 작용하고, 데이터를 수집하고, 데이터를 사용하여 사전 결정된 목표를 달성하기 위해 필요한 작업을 스스로 결정해서 수행할 수 있는 소프트웨어 프로그램
LLM 핵심 인텔리전스 기반으로 구조와 흐름 구축, **AI가 자율적으로 행동하는 능력**을 갖추도록 한다.
- 단순한 챗봇을 넘어 자율적으로 운영됨
- ml, nlp 활용 -> 데이터 분석, 의사결정, 경험 학습

### 주요 구성요소

![스크린샷 2025-04-11 오전 12 39 54](https://github.com/user-attachments/assets/54d99618-1b80-499a-9abc-48a07a7521cd)

### AI Agent 작동 방식
![스크린샷 2025-04-11 오전 12 34 16](https://github.com/user-attachments/assets/75fa200f-4dc9-4856-b2be-ffbf97022efa)
1. 인식 및 데이터 수집
2. 의사결정
3. 작업 실행
4. 학습 및 적응

![스크린샷 2025-04-11 오전 12 42 18](https://github.com/user-attachments/assets/729e898b-c048-47f7-908e-de8ac59d9a55)
- 단순 반응 에이전트(Simple Reactive Agents) : '조건-작용(행동 규칙)' 원리 기반 사전 정의된 규칙과 즉각적인 데이터에 따라 작동하는 가장 간단한 에이전트.
  - 사용자의 대화에서 특정 키워드를 감지할 경우 암호를 초기화하거나, 매일 밤 정해진 시간에 난방 시스템을 켜게 하거나, 고객 챗봇과 같은 일부 시나리오에 적용
- 모델 기반 반응 에이전트(Model-Based Reaction Agents) : 단순히 특정 규칙을 따르는 것이 아니라, 가능성 있는 결과와 결론을 평가하여 결정
  - 로봇 청소기가 방을 청소할 때 가구 등의 장애물을 감지하고 그 주변을 조정하거나, 이미 청소한 영역의 모델을 저장하여 반복되는 청소 루프에 갇히지 않도록 함
- 목표 기반 에이전트(Goal-based Agents) : NLP, 로보틱스 애플리케이션 / 가장 효율적인 경로 선택.
- 유틸리티 기반 에이전트 : 다양한 시나리오와 각각의 효용 가치 또는 이점을 비교한 후, 사용자에게 가장 많은 유용한 안을 선택
  - 고객은 유틸리티 기반 에이전트를 사용하여 가격과 관계없이 이동 시간이 가장 짧은 항공권을 검색, 자율 주행 자동차, 금융거래 등
  - 
- 학습 에이전트(Learning Agents) : 전자 상거래 사이트에서의 개인화된 추천 에이전트, 사기 탐지 시스템
- 계층적 에이전트(Hierarchical Agents) : 상위 에이전트는 복잡한 작업을 작은 작업으로 분해하여 하위 에이전트에 할당한다. 각 에이전트는 독립적으로 실행되며 자신을 감독하는 에이전트에게 진행 상황을 보고한다. 상위 에이전트는 결과를 수집하고, 하위 에이전트가 공동으로 목표를 달성할 수 있도록 하위 에이전트를 조정한다.
-   - 이러한 구조를 통해 기업은 복잡한 다단계 프로세스를 더 간단한 작업으로 나눌 수 있게 되어, 각 AI 에이전트는 하나의 목표와 책임에 집중할 수 있다.

## AI Agent 핵심 요소
LLM = 시스템의 '두뇌' 역할.
외부 리소스, API : AI가 외부 세계와 통신, 데이터 얻기, 특정 작업 수행 시 활용
프롬프트 : LLM의 행동과 인지 과정 지시

### CoT(Chain-of-Thought)
- 정의: LLM이 문제를 단계별로 나누어 논리적으로 해결하도록 유도하는 기법.
- 효과: 복잡한 문제에 대해 더 정확하고 신뢰할 수 있는 답을 생성.
- 관련 연구: Google Brain의 CoT(2022), ReAct(Reasoning + Action).
### 도구와 메모리 사용
- 도구 : 외부 정보에 접근하는 수단(ex: LLM, API, 웹, DB 등)
- 메모리 : 이전 대화나 작업 경험 활용, 더 나은 응답 생성
- 관련 연구 : Meta의 Toolformer, Gorilla(API 선택), CoA(Chain-of-Abstracion)
### 멀티 에이전트 아키텍처
- 정의: 여러 AI Agent가 협업하여 목표를 달성하는 구조.
- 예시: ChatDev - 각 Agent가 CEO, CTO, 개발자 등 역할을 맡아 협력.
- 효과: 복잡한 작업(예: 소프트웨어 개발)을 분업화하고 효율적으로 수행.
![스크린샷 2025-04-11 오전 12 52 22](https://github.com/user-attachments/assets/41731461-6bcd-493d-b5b0-ff531a62a1ee)

![스크린샷 2025-04-11 오전 12 51 46](https://github.com/user-attachments/assets/4dfdc154-5248-4db7-844a-08bc5fd1fb88)
```
[ CoT ]
   ↓           ↘
[ ReAct ]     [ CoA ]
   ↓              ↓
[ Toolformer ]   [ Gorilla ]
        ↘       ↙
      [ 도구 + 메모리 ]
             ↓
      [ 멀티 에이전트 ]
         (ChatDev 등)

```

## Build an Agent


