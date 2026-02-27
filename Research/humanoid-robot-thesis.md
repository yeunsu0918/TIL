---
title: "가정용 휴머노이드 로봇 수용의도 연구 - 논문 진행 현황"
date: 2026-02-27
category: Research
tags: [논문, 박사과정, 휴머노이드, TAM, SEM, ANOVA, 설문조사]
---

# 가정용 휴머노이드 로봇 수용의도 연구 - 논문 진행 현황

## 📌 요약
> 가정용 휴머노이드 로봇의 설명가능성(Transparency)과 적응성(Personalization)이 사용자 수용의도에 미치는 영향을 연구하는 박사 논문. 2x2 실험설계, 400부 설문, PLS-SEM 분석.

## 📝 연구 개요

### 연구 주제
- **가정용 휴머노이드 로봇**의 수용의도(Intention to Use) 영향 요인 분석
- 설명가능성(Transparency) × 적응성(Personalization)의 **2×2 실험설계**
- TAM(기술수용모형) 기반 확장 모형

### 핵심 변수 & 약어
| 약어 | 한국어 | 영어 |
|------|--------|------|
| SP | 사회적 실재감 | Social Presence |
| PE | 지각된 즐거움 | Perceived Enjoyment |
| PEU | 지각된 사용용이성 | Perceived Ease of Use |
| PU | 지각된 유용성 | Perceived Usefulness |
| AT | 태도 | Attitude |
| IU | 사용의도 | Intention to Use |

### 연구 가설
- **H1 (ANOVA):** 설명가능성 × 적응성 상호작용 효과 → AT, PU, PEU, PE, SP, IU
- **H2~H8 (PLS-SEM):** SP→PE→PEU→PU, AT→IU, PU→IU, PEU→IU, PE→IU

### 인과 경로 모형
```
SP → PE → PEU → PU
                    ↘
         AT →        IU  ← PU, PEU, PE
```

## ✅ 진행 현황

### 완료된 작업
- [x] 연구 모형 및 가설 설정
- [x] 2×2 실험 설계 및 시나리오 제작 (A~D)
- [x] 설문지 설계 및 최종본 완성
- [x] 설문 데이터 수집 (400부)
- [x] 데이터 코딩 및 전처리 (v4)
- [x] R 통계분석 코드 작성 (run_ch4_v4.R)
  - ANOVA (일원/이원 분산분석)
  - PLS-SEM (구조방정식모형)
  - MGA (다중집단분석)
- [x] 분석 결과 HTML 뷰어 제작 (chapter_4_viewer_v4.html)
- [x] 검증용 데이터 분석 (run_ch4_verify.R)
- [x] 4장 (실증분석) 본문 작성 (~52KB)
- [x] 5장 (결론) 본문 작성 (~17KB)
- [x] 참고문헌 APA 7th 정리

### 남은 작업
- [ ] 4장 수정안 반영
- [ ] HWP 최종 편집 및 제출

## 📂 프로젝트 구조
```
c:\workspace\휴머노이드 논문\
├── 본문작성\           ← 논문 본체
│   ├── 4장_본문.md     ← 4장 실증분석 (52KB)
│   ├── 5장_결론.md     ← 5장 결론 (17KB)
│   ├── 설문결과_코딩\  ← 400부 데이터
│   └── 참고자료\       ← 참고 문서들
├── 통계분석\           ← R 분석 코드
│   ├── scripts\        ← R 스크립트
│   ├── results_v4\     ← v4 분석 CSV
│   └── figures_v4\     ← 그래프 PNG (~40개)
└── BACKUP\             ← 이전 버전 보관
```

## 💡 느낀 점 / 다음 단계
- Antigravity(Claude)와 협업하여 통계분석 코드 작성 및 결과 해석 진행
- R + PLS-SEM 분석 자동화 파이프라인 구축 경험
- 남은 작업: 4장 수정안 반영 후 HWP 최종 편집
