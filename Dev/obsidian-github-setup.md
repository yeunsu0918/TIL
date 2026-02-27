---
title: "Obsidian + GitHub 지식 관리 셋업"
date: 2026-02-27
category: Dev
tags: [obsidian, github, pkm, til, knowledge-management]
---

# Obsidian + GitHub 지식 관리 셋업

## 📌 요약
> 흩어진 6개 도구(노션, 구글드라이브, 마이박스, 구글킵, 삼성노트, 로컬)를 Obsidian + GitHub 중심으로 통합

## 📝 내용

### 3계층 구조
```
📱 캡처 (구글 킵)  →  🧠 정리 (Obsidian)  →  📦 보관 (GitHub + 구글드라이브)
```

### 정리 방안
| 기존 도구 | 처리 |
|-----------|------|
| 노션 | 필요한 내용만 이동 → 계정 유지 |
| 구글 드라이브 | 유지 — 대용량 파일 전용 |
| 네이버 마이박스 | 폐기 → 구글드라이브로 통합 |
| 구글 킵 | 유지 — 빠른 캡처 전용 |
| 삼성 노트 | 폐기 → 구글 킵으로 통합 |

### Obsidian 필수 플러그인
1. **Obsidian Git** — GitHub 자동 동기화
2. **Templater** — 템플릿 자동 적용
3. **Calendar** — 일일 노트 관리
4. **Dataview** — 노트 쿼리/검색

### 참고 자료
- [Obsidian 공식 사이트](https://obsidian.md)
- [Obsidian Git 플러그인](https://github.com/denolehov/obsidian-git)

## 💡 다음 단계
- Obsidian 앱 설치 후 `c:\workspace\TIL` 폴더를 Vault로 열기
- Obsidian Git 플러그인 설치
- GitHub에 TIL 저장소 생성 후 연결
