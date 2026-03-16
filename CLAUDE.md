# AX Developer Portfolio

## 프로젝트 개요

GitHub Pages로 배포된 정적 포트폴리오 사이트.

- **배포 URL:** https://hwangjoonho.github.io/ax-portfolio/
- **GitHub Repo:** https://github.com/hwangjoonho/ax-portfolio
- **디자인:** 다크 테마 (Pretendard + Space Mono)
- **기술:** 순수 HTML/CSS, JS 최소 사용 (IntersectionObserver만)

## 파일 구조

```
portfolio/
├── index.html              ← 메인 포트폴리오 (전체 섹션 포함)
└── projects/
    ├── rag.html             ← RAG 시스템 상세 (다크 테마)
    ├── ocr.html             ← OCR 시스템 상세 (라이트 테마)
    ├── gitops.html          ← GitOps CI/CD 상세 (다크 테마, 신규 제작)
    ├── babmokja.pdf         ← 과거 프로젝트 - 업체 파트 추출본
    └── tripweb.pdf          ← 과거 프로젝트 - 마이페이지 파트 추출본
```

## index.html 섹션 구성

| # | 섹션 ID | 내용 |
|---|---------|------|
| 1 | `hero` | 타이틀, 소개, 기술 뱃지 |
| 2 | `about` | About Me 역량 소개 |
| 3 | `career` | 경력 타임라인 (4개사) |
| 4 | `tech` | Tech Stack 8개 카테고리 카드 |
| 5 | `projects` | 주요 프로젝트 3개 카드 → 상세 페이지 링크 |
| 6 | `certifications` | 자격증 5개 |
| 7 | `past-projects` | 과거 교육 프로젝트 2개 → PDF 링크 |

## 프로젝트 상세 페이지

### rag.html (RAG 파이프라인)
- **원본:** `RAG_foli/XT_RAG_파이프라인 계획서.html` 기반
- **테마:** 다크 (Pretendard 폰트)
- **내용:** 시스템 아키텍처, 성과 지표, 5-Phase 청킹, Hybrid Search, ADK Agent 연동, 기술 의사결정
- 상단에 "← Portfolio" 네비게이션 바 추가됨

### ocr.html (OCR 파이프라인)
- **원본:** `paddleOCR_foli/portfolio.html` 기반
- **테마:** 라이트 (Inter 폰트)
- **내용:** MCP 프로토콜 한계 우회, tmpfs 공유 볼륨, 5개 문제 해결 과정, Quality Gate, 전처리 파이프라인
- 상단에 "← Portfolio" 네비게이션 바 추가됨

### gitops.html (GitOps CI/CD)
- **테마:** 다크 (Pretendard 폰트)
- **내용:** E2E Flow, Frontend/Backend 파이프라인, 인프라 구성 6개, 핵심 기능 6개, ci-config.yaml 예시
- 신규 제작 (04_GitOps_프로젝트_상세.md 기반)

## 경력 정보 (Career 섹션)

### (주)엑스티(XT) — 대리 | 2024.10 ~ 현재
- 사내 자체 AI 서버 개발 및 셀프호스팅 (vLLM, Ollama, TensorRT)
- 사내 쿠버네티스(K3s) 환경 구축 및 운영
- RAG 파이프라인 전체 설계 및 구축 (Weaviate, Hybrid Search, 5-Phase 청킹)
- Enterprise OCR 시스템 구축 (PaddleOCR-VL + MCP 프로토콜 한계 우회)
- GitOps CI/CD 파이프라인 설계 (Jenkins + ArgoCD + Kustomize)
- 초록우산 애플리케이션 백엔드 개발
- 서버 인프라 구축 — Proxy(Nginx) / Frontend(Apache, Nginx) / Backend(Tomcat)
- Hoppscotch API 테스트 도구 셀프호스팅
- 테스트 자동화 시스템 총괄
- MCP 기반 AI 도구 연동 (Gemini CLI, Claude Code)

### (주)에듀에이아이 — 주임/계장 | 2023.05 ~ 2024.10
- KERIS 프로젝트 — 개발환경, MVC, React, AWS, Git, SSL, 배포
- Docker 클라우드 관리, AWS VPC/S3/로드밸런싱
- 자연어 처리 API, Chatbot 테스트 개발

### 엠싱크 — 사원 | 2023.01 ~ 2023.04
- 교촌 앱 추가 개발 및 오류 처리

### 젠솔소프트 — 사원 | 2021.09 ~ 2022.11
- WAS/DB, 형상관리 서버 관리, 네트워크 작업

## 자격증

| 자격증 | 취득일 | 발행처 |
|--------|--------|--------|
| 정보처리기사 | 2024.05 | 한국산업인력공단 |
| 컴퓨터활용능력 1급 | 2019.06 | 대한상공회의소 |
| 워드프로세서 1급 | 2012.06 | 대한상공회의소 |
| ITQ 아래한글 1급 | 2012.02 | 한국생산성본부 |
| ITQ 파워포인트 1급 | 2012.02 | 한국생산성본부 |

## 과거 프로젝트 PDF

| 파일 | 프로젝트 | 담당 파트 | 원본 추출 |
|------|----------|----------|----------|
| `babmokja.pdf` | 배달/픽업/예약 플랫폼 (Semi, 2021) | 업체 기능 전체 | 원본 56p 중 21p 추출 (소개 1-10 + 황준호 28-38) |
| `tripweb.pdf` | 제주도 여행 플랜 공유 (Final, 2021) | 이용자 마이페이지 전체 | 원본 45p 중 21p 추출 (소개 1-14 + 황준호 38-44) |

## 디자인 규칙

### 컬러 (다크 테마)
```
--bg-primary: #0a0f1e
--bg-secondary: #0f1629
--bg-card: #151d30
--border: #1e2d4a
--text-primary: #e8edf5
--text-secondary: #8b9dc3
--accent-blue: #3b82f6
--accent-cyan: #06b6d4
--accent-violet: #8b5cf6
--accent-emerald: #10b981
--accent-amber: #f59e0b
```

### 폰트
- 본문: Pretendard (CDN)
- 모노: Space Mono (Google Fonts)

### 배경 패턴
```css
radial-gradient(circle, rgba(59,130,246,0.06) 1px, transparent 1px);
background-size: 32px 32px;
```

## 배포 방법

```bash
# portfolio/ 디렉토리에서
git add -A
git commit -m "설명"
git push
# GitHub Pages가 자동 빌드 (legacy mode, main branch, / root)
```

## 작업 시 주의사항

- 각 HTML은 **단일 파일** (CSS 내장, 외부 의존성 = Google Fonts만)
- `ocr.html`만 **라이트 테마**, 나머지는 **다크 테마**
- 프로젝트 상세 페이지에는 상단 고정 "← Portfolio" 네비게이션 바 있음
- PDF 파일은 본인(황준호) 담당 파트만 추출된 것
- 원본 가이드 파일: `/Users/xtaidev/AI/foli/portfolio-guide/` (로컬 전용, repo 미포함)
