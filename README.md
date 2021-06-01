# Portfolio_Semin
[Semin's Level up Stage](https://seminoh.oopy.io/)

---
## 1. (NLP) Dialogue State Tracking 
[자세히 보기](https://seminoh.oopy.io/810be715-7290-47e8-83cf-8fcfca026c4d)
[팀 깃헙](https://github.com/bcaitech1/p3-dst-teamed-st)
### 1. 프로젝트 요약

#### 1-1 대회 설명

- **TOD는 시나리오 데이터 기반으로 수행**된다. 이를 잘 수행하기 위해서는 유저가 원하는 바를 제대로 파악해야하고, **DST**가 이 역할을 담당한다.
- 유저가 서울을 여행을 하면서 경험할 **시나리오 기반 데이터셋인 Wizard of Seoul** 의 각 대화에서 정확한 정보를 파악하는 것이 프로젝트의 목표이다.

#### 1-2 데이터

- 본 프로젝트의 목표는 시나리오의 각 turn에서의 정보를 정확히 발견해내는 것이다.

#### EX)

- input: ["안녕하세요.", "네. 안녕하세요. 무엇을 도와드릴까요?", "서울 중앙에 위치한 호텔을 찾고 있습니다. 외국인 친구도 함께 갈 예정이라서 원활하게 인터넷을 사용할 수 있는 곳이 었으면 좋겠어요."]
- output: **Dialogue State**
    - ["숙소-지역-서울 중앙", "숙소-인터넷 가능-yes"]



## 2. Relation Extraction
[자세히 보기](https://www.notion.so/torreira/Klue-Wrap-up-Report-67c41887ee4b45ea831b1fe1a97175bc)
[깃헙]()
### 1. 프로젝트 요약

#### 1-1 대회 설명

- 이번 대회에서는 문장, 엔티티, 관계에 대한 정보를 통해 ,문장과 엔티티 사이의 관계를 추론하는 모델을 학습시킵니다.
- 이를 통해 우리의 인공지능 모델이 엔티티들의 속성과 관계를 파악하며 개념을 학습할 수 있습니다.
- 우리의 model이 정말 언어를 잘 이해하고 있는 지, 평가해 보도록 합니다.

#### 2-2 데이터

- 입력 문장이 들어오고, 두개의 entity가 어떤 관계인지 예측한다.
- input: sentence, entity1, entity2 의 정보를 입력으로 사용 합니다

#### EX)

```
sentence: 오라클(구 썬 마이크로시스템즈)에서 제공하는 자바 가상 머신 말고도 각 운영 체제 개발사가 제공하는 자바 가상 머신 및 오픈소스로 개발된 구형 버전의 온전한 자바 VM도 있으며, GNU의 GCJ나 아파치 소프트웨어 재단(ASF: Apache Software Foundation)의 하모니(Harmony)와 같은 아직은 완전하지 않지만 지속적인 오픈 소스 자바 가상 머신도 존재한다.

entity 1: 썬 마이크로시스템즈
entity 2: 오라클

relation: 단체:별칭
```

- output: relation 42개 classes 중 1개의 class를 예측한 값




 
 
