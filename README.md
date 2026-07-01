# 바이브 코딩 첫걸음 · 장대현중고등학교

AI와 대화하며 나만의 웹앱을 만들고 인터넷에 배포하는 **중·고등 원데이 코딩 수업**(3시간) 자료입니다.
강의 **슬라이드**와 **스타터 패키지**가 한 저장소에 들어 있어요.

- 📊 **강의 슬라이드(웹):** https://aightlabs.github.io/jdh-school-vibe-coding/
- 📦 **저장소:** https://github.com/AightLabs/jdh-school-vibe-coding
- 🧰 **스타터 가이드:** [STARTER-GUIDE.md](./STARTER-GUIDE.md)

## 📂 구성
| 경로 | 내용 |
|---|---|
| `index.html` | **강의 슬라이드** (열면 바로 실행 · ← → 이동 · 코드 복사 · 인쇄 · 한국어/中文 토글) |
| `starters/game/` | **게임 스타터** — Phaser 3 별 받기 게임 + prd.md + context.md |
| `starters/nongame/` | **비게임 스타터** — Tailwind + Vanilla JS 소개 페이지 + prd.md + context.md |
| `STARTER-GUIDE.md` | 스타터 준비·사용·배포 정리 문서 |

## 🧑‍🎓 학생용 빠른 시작
1. 이 저장소를 받기 — 초록 **Code → Download ZIP**, 또는
   ```
   git clone https://github.com/AightLabs/jdh-school-vibe-coding.git
   ```
2. `starters/`에서 원하는 스타터 폴더를 **내 새 폴더로 복사** → VS Code로 열기
3. `index.html`을 브라우저/Live Server로 확인, `prd.md`를 내 기획으로 채우기
4. **Copilot Chat**에 하나씩 부탁하며 키우기
5. **Source Control → Commit → Publish to GitHub** → **Settings → Pages → main /(root)** 로 내 주소 공개
   → 자세한 단계는 [STARTER-GUIDE.md](./STARTER-GUIDE.md)

## 🖥 강의 슬라이드 보기 / 배포
- 로컬: `index.html`을 브라우저로 열기
- 웹 공개(GitHub Pages): **Settings → Pages → Branch: `main` /(root) → Save** → https://aightlabs.github.io/jdh-school-vibe-coding/
- **인쇄/PDF 유인물:** 상단 **🖨 인쇄** → 한 슬라이드가 한 페이지. 언어 토글을 中으로 두고 인쇄하면 중국어 유인물

## 🧭 슬라이드 목차
0. 시작 · 오늘 배울 것 (+ 링크/QR)
1. 바이브 코딩이란?
2. 기초 CS 지식 (언어 · GUI/CLI · 웹 3종 · Git)
3. 개발환경 설치 (VS Code · Git · Copilot) + 스타터 clone · 미리보기
4. 프롬프트 엔지니어링
5. 컨텍스트 엔지니어링
6. 기획 · PRD → 목업 → MVP
7. 개발 · MVP 만들기
8. 배포 · 여러 방법 (GitHub Pages 외)
9. 이후 3일 & 부록 (문제 해결 · 치트시트 · 용어 사전 · Markdown 문법)
＋ 교양 · 더 알면 좋은 것 (서버·클라우드 · 도메인/IP/DNS · 프론트/백엔드 · DB · API · AI/LLM · 오픈소스 · 버그)

## ⚙️ 스택
- 강의 슬라이드: 순수 HTML/CSS/JS (Pretendard · JetBrains Mono · Noto Sans SC) — 외부 로컬 의존성 없음
- 게임 스타터: Phaser 3 · 비게임 스타터: Tailwind CSS + Vanilla JS
- 배포: GitHub Pages
