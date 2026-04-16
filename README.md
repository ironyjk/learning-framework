# Learning Framework

성인 학습·지식 관리 메타 라우터 + 프레임워크 컬렉션. 인지과학·교육심리학 연구 기반 12개 프레임워크를 하나의 라우팅 레이어에 묶는다.

## 설계 원칙

1. **연구 기반 > 자기계발 서사** — "천재들의 습관", "○○ 법칙" 같은 과장 대신 실증 연구(Ebbinghaus·Roediger·Karpicke·Dunlosky·Ericsson·Bjork·Cepeda)에서 출발. 근거 약한 주장(학습 유형 VAK, 우뇌/좌뇌, 속독, 10,000시간 법칙, 1분 기억법 등)은 포함하지 않거나 명시적으로 교정.
2. **도구가 아니라 원리** — Obsidian·Notion·Anki·Logseq·Roam 같은 특정 도구 홍보 대신 원리 중심. 도구는 중립적으로만 언급.
3. **단일 만능 프레임워크 없음** — 지식 포착은 Zettelkasten, 기억은 Spaced Repetition, 이해 검증은 Feynman 식으로 *조합*하는 것을 전제.
4. **과적용 경고 포함** — 각 프레임워크가 틀리거나 해로울 때를 명시.
5. **Desirable difficulty 일관 적용** — Bjork. 편한 학습(하이라이트·재독·요약 소비)은 대부분 덜 학습된다. 주관과 결과는 반대.
6. **자기주도 ≠ 고립** — 코치·스터디·AI·인강을 외부 피드백 채널로 통합. 혼자서는 blind spot이 굳는다.
7. **한국 학습 맥락 내장** — 수능·공무원·자격증(공인중개사·CPA·PMP)·회독·오답노트·N수·인강 문화 등 한국 학습자 현장을 사례로.

## 구조

```
learning-framework/
├── SKILL.md                   # 메타 라우터 — 상황 → 프레임워크 선택
├── zettelkasten/              # Luhmann 아토믹 노트·연결
├── second-brain-para/         # Tiago Forte PARA·CODE
├── evergreen-notes/           # Andy Matuschak 개념 지향·지속 편집
├── spaced-repetition/         # Ebbinghaus 망각곡선·SM-2
├── active-recall/             # Roediger·Karpicke 테스팅 효과
├── feynman-technique/         # 설명으로 이해 검증
├── interleaving/              # Bjork 섞어 학습
├── deliberate-practice/       # Ericsson 의도적 연습
├── chunking/                  # Miller 청킹·전문가 지각
├── deep-work/                 # Cal Newport 깊은 일
├── pomodoro-and-focus/        # Cirillo 25/5 + attention residue
└── metalearning/              # Oakley + Young 메타 학습
```

## 사용

```
/learn <상황 설명>
```

메타 라우터가 목적(시험/스킬/지식 축적)과 제약(시간·도구)을 분류하고, 관련 프레임워크 1~3개를 선택해 Skill 툴로 실행·합성.

## 범위 바깥

- 아동·청소년 교육 (→ `parenting`, `udl`, `pbl` 등)
- 협상·커뮤니케이션 학습법 (→ `howtotalk`)
- 심리치료·정서 학습 (→ `counsel`)
- 조직 학습·팀 스킬 (→ `team-topologies`)

이 레포는 성인이 스스로 학습하고, 지식을 축적하고, 전문성을 쌓는 맥락에 초점.

## 면책

이 레포는 학습 설계 보조 도구다. 공인 시험·자격증 준비·임상 영역(의대·법대 등)은 별도 전략이 필요할 수 있다.
