# 🤝 AI Handoff Template

Claude와 Codex(또는 다른 AI)를 번갈아 사용할 때
**작업 맥락을 끊김 없이 유지**하기 위한 범용 인계 파일 시스템입니다.

## 📁 폴더 구조

```
your-project/
├── CLAUDE.md              ← Claude용 고정 지침 (프로젝트 루트)
├── AGENTS.md              ← Codex용 고정 지침 (프로젝트 루트)
└── .ai-handoff/
    ├── README.md          ← 이 파일
    ├── HANDOFF.md         ← 프로젝트 현황 (기술 스택, 구조, 브랜치)
    ├── TODO.md            ← 할 일 목록 (완료 / 진행 중 / 예정)
    ├── DECISIONS.md       ← 기술적 결정 사항 및 주의사항
    ├── SESSION_LOG.md     ← 최신 세션 작업 로그
    ├── START_PROMPTS.md   ← AI 세션 시작 시 사용할 프롬프트 모음
    └── archive/           ← 오래된 세션 로그 월별 보관
```

## 🚀 새 프로젝트에 적용하는 방법

```
1. 이 템플릿 폴더를 새 프로젝트 루트에 복사
2. HANDOFF.md에 프로젝트 정보 작성
3. TODO.md에 할 일 목록 작성
4. CLAUDE.md / AGENTS.md 프로젝트에 맞게 수정
5. 세션 시작 시 START_PROMPTS.md의 프롬프트 사용
```

## 🔄 세션 종료 시 업데이트 규칙

| 파일 | 업데이트 시점 |
|------|-------------|
| `TODO.md` | 작업 완료/추가될 때마다 |
| `SESSION_LOG.md` | 매 세션 종료 전 |
| `DECISIONS.md` | 새로운 기술적 결정이 생길 때 |
| `HANDOFF.md` | 프로젝트 구조나 스택이 바뀔 때 |
| `archive/` | SESSION_LOG가 너무 길어질 때 월별로 이동 |
