---
title: "CMUX vs DMUX 비교"
date: 2026-02-27
category: AI
tags: [agent-orchestration, cmux, dmux, mux, langgraph, crewai]
---

# CMUX vs DMUX 비교

## 요약
CMUX(Mux)는 GUI 기반 에이전트 병렬 실행 관리 도구, DMUX는 CLI(tmux) 기반 에이전트 분산 실행 도구. 실제 오케스트레이션(작업 분배, 의사결정)에는 별도 프레임워크(LangGraph, CrewAI 등)가 필요하다.

## 내용

### CMUX (Coding Agent Multiplexer, 현재 Mux)
- Coder Technologies 개발, GUI 데스크톱 앱
- 여러 AI 코딩 에이전트를 병렬로 실행, 격리된 워크스페이스 제공
- Claude Code, Codex, Gemini CLI 등 터미널 기반 에이전트 지원
- macOS 기본, Linux/Windows 프리빌드 제공

### DMUX (CLI Agent Multiplexer)
- tmux + git worktree 기반 CLI 도구
- `npm install -g dmux`로 설치
- AI 기반 브랜치 명명, 커밋 메시지 자동 생성

### 핵심 차이

| 항목 | CMUX (Mux) | DMUX |
|------|-----------|------|
| 인터페이스 | GUI | CLI (tmux) |
| Windows 지원 | 제한적 | WSL 필요 |
| 적합 사용자 | GUI 선호 | 터미널 파워유저 |

### 오케스트레이션 프레임워크

| 프레임워크 | 특징 | 설치 |
|-----------|------|------|
| LangGraph | 그래프 기반, 복잡한 워크플로우 | `pip install langgraph` |
| CrewAI | 역할 기반 팀, 진입장벽 낮음 | `pip install crewai` |
| AutoGen | 대화 기반, Microsoft 개발 | `pip install autogen-agentchat` |

## 참고 자료
- [Mux GitHub](https://github.com/coder/mux)
- [dmux GitHub](https://github.com/coder/dmux)
- [CrewAI Docs](https://docs.crewai.com)

## 다음 단계
- CrewAI 설치 후 간단한 에이전트 오케스트레이션 실습
- [[obsidian-github-setup]]
