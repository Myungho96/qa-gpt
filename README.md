# QA-GPT: AI 기반 IT SI 산출물 자동 품질검토 및 개선 플랫폼

**QA-GPT**는 AI를 활용하여 IT SI 프로젝트의 산출물을 자동으로 검토하고 개선하는 플랫폼입니다.

## 🎯 핵심 기능

산출물 업로드 시 다음 3가지를 **자동으로 생성**합니다:

1. **품질검토 결과서** — ERROR/WARNING/OK 3단계 분류 및 0~100점 품질 점수
2. **AI 개선 원본 파일** — 결함을 직접 수정한 산출물 새 버전 ([개선] 태그 표시)
3. **개선 비교표** — Before/After 항목별 비교 및 개선 사유 문서화

## 📋 문서

- **[QA-GPT-PRD.md](./QA-GPT-PRD.md)** — 상세 PRD (Problem, Solution, User Stories, Implementation, Testing, Out of Scope)
- **[spec.md](./spec.md)** — 초기 스펙 문서
- **[CLAUDE.md](./CLAUDE.md)** — Claude Code 설정 (Agent Skills)

## 🛠️ Agent Skills

이 프로젝트는 Matt Pocock의 engineering skills와 호환됩니다:

- **Issue tracker**: GitHub Issues
- **Triage labels**: 5개의 표준 분류 라벨
- **Domain docs**: Single-context (CONTEXT.md + docs/adr/)

자세한 내용은 [CLAUDE.md](./CLAUDE.md)의 "Agent skills" 섹션을 참고하세요.

## 📁 프로젝트 구조

```
.
├── QA-GPT-PRD.md                 # 상세 PRD 문서
├── spec.md                       # 초기 스펙
├── CLAUDE.md                     # Claude Code 설정
├── docs/
│   └── agents/                   # Agent skills 설정
│       ├── issue-tracker.md      # GitHub Issues 사용 가이드
│       ├── triage-labels.md      # 분류 라벨 정의
│       └── domain.md             # 도메인 문서 구조
└── README.md                     # 이 파일
```

## 🚀 개발 기간

- **1개월 해커톤** — MVP 범위로 집중 개발
  - Excel (.xlsx) 포맷 개선 원본 지원
  - 주요 산출물 유형 자동 인식 (요구사항정의서, 설계서, WBS, 테스트케이스 등)
  - 프로젝트 단계별 품질 기준 적용

## 💡 기대 효과

| 지표 | 현행 | QA-GPT |
|------|------|--------|
| **검토 소요 시간** | 수일 | 수 분 |
| **24시간 검토** | ✗ | ✓ |
| **검토 비용** | 제3자 QA 외부비용 | 자동화로 대폭 감소 |
| **재검증** | 높은 비용 | 무제한(자동) |
| **검수 대응** | 분쟁 위험 | 문서화된 근거 |

## 📧 Contact

- **팀명**: QA-GPT팀
- **이메일**: facade960409@gmail.com
