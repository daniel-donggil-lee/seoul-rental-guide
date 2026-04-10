# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 프로젝트 개요

아버지(1951년생, 만 74세) 서울 장기임대 아파트 입주 가이드.
공공임대 유형 비교 + 아버지 실제 상황 분석 + 당첨 확률 분석을 담은 단일 HTML.

## 파일 구조

```
seoul-rental-guide/
└── index.html    # 메인 가이드 (SSOT — 이 파일만 수정)
```

## 배포

- GitHub Pages: `https://daniel-donggil-lee.github.io/seoul-rental-guide/`
- Push 시 토큰 삽입 방식 사용 (403 방지):
  ```bash
  TOKEN=$(/opt/homebrew/bin/gh auth token)
  git remote set-url origin "https://daniel-donggil-lee:${TOKEN}@github.com/daniel-donggil-lee/seoul-rental-guide.git"
  git push origin main
  ```

## 아버지 상황 요약 (2026년 4월 기준)

| 항목 | 내용 |
|------|------|
| 나이 | 1951년생, 만 74세 (2026년 중 만 75세) |
| 소득 | 부부 합산 473만원 (아버지 314 + 어머니 159) |
| 주택 | 보유 (시세 2.1억, 유주택) |
| 차량 | 산타페 15년 |
| 전입 | 서울 전입 예정 |

## 신청 가능 프로그램 (유주택 기준)

| 프로그램 | 가능 여부 | 소득 기준 |
|---------|---------|---------|
| 국민임대 | ✅ | 80% = 516만, 통과 |
| 통합공공임대 | ✅ | 100% = 645만, 통과 |
| 행복주택 고령자 | ✅ | 100% = 645만, 통과 |
| 장기전세(시프트) | ✅ | 120% = 774만, 통과 |
| 영구임대 | ❌ | 50% = 323만, 초과 |

> 유주택이어도 공공임대는 신청 가능. 단, 입주 시 기존 주택 처분 조건 있음.

## 배점 전략

- 현재 4/6점 (나이 2점 + 거주기간 2점)
- **2026년 만 75세 생일 이후 신청 시 나이 3점으로 상승** → 5/6점
- 서울 전입 후 5년 경과 시 거주기간 3점 → 최고 6점

## 추천 단지

강동구 고덕강일(고덕온빛채 등) — 서울 외곽 중 경쟁률 낮고 신축 많음.
노원·도봉·강북·중랑·구로·은평구도 외곽 단지로 경쟁률 낮은 편.
