---
title: "가정용 휴머노이드 로봇 수용의도 연구 - 논문 진행 현황"
date: 2026-02-27
category: Research
tags: [thesis, humanoid, TAM, SEM, ANOVA, survey]
---

# 가정용 휴머노이드 로봇 수용의도 연구

## 요약
설명가능성(Transparency)과 적응성(Personalization)이 가정용 휴머노이드 로봇 수용의도에 미치는 영향. 2x2 실험설계, 400부 설문, PLS-SEM 분석.

## 내용

### 연구 개요
- 2x2 실험설계: 설명가능성(T) x 적응성(P)
- TAM(기술수용모형) 기반 확장 모형
- 설문 400부 수집 완료

### 핵심 변수

| 약어 | 한국어 | 영어 |
|------|--------|------|
| SP | 사회적 실재감 | Social Presence |
| PE | 지각된 즐거움 | Perceived Enjoyment |
| PEU | 지각된 사용용이성 | Perceived Ease of Use |
| PU | 지각된 유용성 | Perceived Usefulness |
| AT | 태도 | Attitude |
| IU | 사용의도 | Intention to Use |

### 연구 가설
- H1 (ANOVA): T x P 상호작용 효과 → AT, PU, PEU, PE, SP, IU
- H2~H8 (PLS-SEM): SP→PE→PEU→PU, AT→IU, PU→IU, PEU→IU, PE→IU

### 인과 경로
```
SP → PE → PEU → PU
                    ↘
         AT →        IU  ← PU, PEU, PE
```

## 진행 현황

### 완료
- 연구 모형/가설 설정, 실험 설계, 설문지 완성
- 데이터 수집(400부) 및 코딩/전처리(v4)
- R 통계분석 (ANOVA, PLS-SEM, MGA)
- HTML 결과 뷰어 제작 (chapter_4_viewer_v4.html)
- 4장 실증분석 본문 (~52KB), 5장 결론 본문 (~17KB)
- 참고문헌 APA 7th 정리

### 남은 작업
- 4장 수정안 반영
- HWP 최종 편집 및 제출

## 참고 자료
- 프로젝트 위치: `c:\workspace\휴머노이드 논문\`
- 분석 코드: `통계분석/scripts/run_ch4_v4.R`
