# 바이브 코딩 첫걸음 · 장대현중고등학교

AI와 대화하며 나만의 웹앱을 만들고 인터넷에 배포하는 **중·고등 원데이 코딩 수업**(3시간) 자료입니다.
이 저장소 하나에 **강의 슬라이드**와 **스타터 패키지**가 함께 들어 있어요. `git clone` 하면 그대로 시작 세트가 됩니다.

## 📂 구성
| 경로 | 내용 |
|---|---|
| `index.html` | **강의 슬라이드** (열면 바로 실행 · 키보드 ← → 이동 · 코드 복사 · 인쇄 가능) |
| `starters/game/` | **게임 스타터** — Phaser 3 별 받기 게임 + 전용 PRD |
| `starters/nongame/` | **비게임 스타터** — Tailwind + Vanilla JS 소개 페이지 + 전용 PRD |

## 🧑‍🎓 학생용 — 이렇게 시작해요
1. 이 저장소를 내려받아요. (초록 **Code → Download ZIP**, 또는)
   ```
   git clone https://github.com/OWNER/REPO.git
   ```
2. `starters/` 에서 원하는 스타터 폴더를 골라 **내 작업 폴더로 복사**해요.
   - 게임을 만들고 싶다 → `starters/game`
   - 소개/서비스 페이지를 만들고 싶다 → `starters/nongame`
3. 그 폴더의 `index.html` 을 브라우저로 열어 **바로 확인**하고, `prd.md` 를 내 기획으로 채워요.
4. **Copilot Chat** 에게 하나씩 부탁하며 키워요. (자세한 방법은 슬라이드 참고)
5. VS Code **Source Control → Commit → Publish to GitHub** 로 올리고,
   **Settings → Pages → main /(root)** 로 켜면 `https://내아이디.github.io/내저장소/` 로 공개돼요.

## 🖥 강의 슬라이드 보기 / 배포
- 로컬에서 보기: `index.html` 을 브라우저로 열기.
- 웹으로 공개(GitHub Pages): 이 저장소 **Settings → Pages → Branch: `main` /(root) → Save** → 몇 분 뒤 아래 주소에서 공개됩니다.
  ```
  https://OWNER.github.io/REPO/
  ```
- **인쇄/PDF 유인물:** 슬라이드 상단의 **🖨 인쇄** 버튼 → 한 슬라이드가 한 페이지로 인쇄돼요. (언어 토글을 中으로 두고 인쇄하면 중국어 유인물)

## 🧭 강의 목차 (슬라이드)
0. 시작 · 오늘 배울 것
1. 바이브 코딩이란?
2. 기초 CS 지식 (언어 · GUI/CLI · 웹 3종 · Git)
3. 개발환경 설치 (VS Code · Git · Copilot)
4. 프롬프트 엔지니어링
5. 컨텍스트 엔지니어링
6. 기획 · PRD → 목업 → MVP
7. 개발 · MVP 만들기
8. 배포 · 여러 방법 (GitHub Pages 외)
9. 이후 3일 & 부록 (문제 해결 · 치트시트 · 용어 사전)

## ⚙️ 스택
- 강의 슬라이드: 순수 HTML/CSS/JS (Pretendard · JetBrains Mono)
- 게임 스타터: Phaser 3
- 비게임 스타터: Tailwind CSS + Vanilla JS
- 배포: GitHub Pages
