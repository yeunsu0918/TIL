---
title: TIL 작성 가이드
updated: 2026-02-27
---

# TIL 작성 가이드

AI 도구든 사람이든 TIL에 글을 쓸 때 이 문서를 먼저 읽고 따른다.
(참고: jbranchaud/til, simonw/til, Obsidian 커뮤니티 컨벤션 기반)

---

## 글 유형 구분

| 유형 | 위치 | 파일명 | 예시 |
|------|------|--------|------|
| 정보/학습 | 주제 폴더 (AI/, Dev/ 등) | `주제명.md` | `AI/cmux-vs-dmux.md` |
| 일지/기록 | Daily/ | `YYYY-MM-DD.md` | `Daily/2026-02-27.md` |
| 추적/로그 | 주제 폴더 | `주제명.md` (누적 갱신) | `Health/health-tracker.md` |

- 정보성 글은 날짜가 아니라 **주제**가 파일명이다.
- 날짜는 파일 안 frontmatter의 `date`에만 기록한다.
- 같은 주제를 나중에 보강하면 `updated` 필드를 갱신한다.

## 파일명 규칙

- 영문 소문자, 단어 구분은 하이픈(`-`)
- 한글 파일명 금지 (Git/GitHub 호환성)
- 짧고 명확하게

```
좋은 예: cmux-vs-dmux.md, pls-sem-basics.md
나쁜 예: CMUX vs DMUX 비교.md, 2026-02-27-cmux.md, 새파일.md
```

## Frontmatter

```yaml
---
title: "제목 (한글 OK)"
date: 2026-02-27
updated: 2026-02-27        # 수정 시에만 추가
category: AI               # 폴더명과 동일
tags: [agent, orchestration]
---
```

필수: `title`, `date`, `category`
선택: `updated`, `tags`

## 본문 구조

```markdown
# 제목

## 요약
핵심을 한두 줄로.

## 내용
본문. 소제목은 ### 사용.

## 참고 자료
- 출처, 링크

## 다음 단계
후속 작업, 떠오른 생각 (없으면 생략)
```

## 작성 톤

- 이모지는 최소한. 제목이나 섹션 헤더에 하나 정도만 허용.
- 표(table)는 비교할 때만. 남용 금지.
- 한 파일 = 한 주제. 500줄 넘으면 분리 고려.
- 코드 블록은 언어 명시.
- 다른 노트 참조: `[[파일명]]` (Obsidian 링크).

## 폴더 구조

```
TIL/
├── README.md          ← 목차 (주기적 갱신)
├── STYLE_GUIDE.md     ← 이 문서
├── _templates/        ← 템플릿
├── AI/                ← AI, LLM, 에이전트
├── Research/          ← 논문, 통계, 학술
├── Dev/               ← 개발, 도구
├── Health/            ← 건강, 운동
├── Ideas/             ← 사업, 콘텐츠 기획
├── Life/              ← 시간관리, 일상
└── Daily/             ← 일일 기록 (날짜 파일명)
```

새 카테고리가 필요하면 폴더 추가. 빈 폴더는 만들지 않는다.

## AI 도구에게 요청할 때

```
"이거 TIL에 저장해줘" → AI가 STYLE_GUIDE.md 참고해서 작성
"Research에 정리해줘" → 해당 폴더에 저장
"STYLE_GUIDE.md 따라서 써줘" → 포맷 준수 강제
```

## 커밋 메시지 규칙

```
Add: 새 글 추가       예) Add: cmux-vs-dmux 비교
Update: 기존 글 수정  예) Update: thesis progress 현황 갱신
Daily: 일일 기록      예) Daily: 2026-02-27
```
