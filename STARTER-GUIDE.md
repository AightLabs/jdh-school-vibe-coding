# 🧰 스타터 준비 & 사용 가이드

이 문서 하나로 **스타터가 무엇인지, 무엇이 들어 있는지, 어떻게 시작하고 배포하는지**를 정리했어요.
(강의 슬라이드: https://aightlabs.github.io/jdh-school-vibe-coding/ · 저장소: https://github.com/AightLabs/jdh-school-vibe-coding)

---

## 1. 스타터란?
"처음부터 아무것도 없는 백지"가 아니라, **기획서·규칙·에셋이 갖춰진 빈 뼈대(스켈레톤)**에서 시작하는 시작 세트예요.
먼저 `prd.md`에 기획을 채우고, OpenCode에게 말하며 `index.html`을 만들어 나갑니다.

두 가지가 있어요:

| 스타터 | 만들 것 | 스택 | 폴더 |
|---|---|---|---|
| 🎮 게임 | 웹게임 (별 받기 등) | **Phaser 3** | `starters/game/` |
| 🌟 앱 | 소개/서비스 페이지 | **Tailwind CSS + Vanilla JS** | `starters/app/` |

## 2. 스타터 폴더에 들어 있는 것 (공통)
| 파일 | 역할 |
|---|---|
| `AGENTS.md` | **AI(OpenCode)가 자동으로 읽는 규칙·안내** |
| `prd.md` | **기획 템플릿** — 무엇을 만들지 정리 (뼈대 + 채운 예시) |
| `design.md` | 🎨 색·폰트·스타일(게임은 게임 느낌) 가이드 — AI가 읽음 |
| `context.md` | **기억 파일** — "다음에 할 일"을 적어두는 곳 (컨텍스트 관리) |
| `index.html` | **빈 뼈대** — 여기에 내 앱/게임이 만들어져요 (HTML 단일 파일) |
| `README.md` | 그 스타터 전용 사용법 |
| `assets/` | 아이콘·스프라이트 등 · `RESOURCES.md`(무료 출처) |

> 공통 특징: **빈 뼈대에서 시작** → `prd.md` 채우고 AI로 완성 → **HTML 파일 하나로 된 웹앱** + **GitHub Pages 배포**(커밋 → 푸시 → Pages).

## 3. 준비물 (수업 전/중)
- **GitHub 계정** (사전 가입 완료)
- **VS Code** · **Git** 설치 (슬라이드 CH3 참고)
- **Node.js + OpenCode** + 모델(Zen 무료) — AI 코딩 도구 (설치: [SETUP-OpenCode-Zen.md](./SETUP-OpenCode-Zen.md))
- (권장) VS Code 확장 **Live Server** — 결과를 바로 미리보기

## 4. 시작하기 — 3단계

### ① 내려받기 (둘 중 하나)
- **방법 A · ZIP (가장 쉬움):** 저장소에서 초록 **Code → Download ZIP** → 압축 풀기
- **방법 B · git clone:**
  ```
  git clone https://github.com/AightLabs/jdh-school-vibe-coding.git
  ```

### ② 내 폴더로 복사 후 열기
- `starters/game` 또는 `starters/app` 폴더를 **바탕화면의 새 폴더**(영어 이름, 예: `my-game`)로 복사
- VS Code에서 그 새 폴더를 **File → Open Folder**
- `index.html` 열어보기 — 지금은 **안내만 뜨는 빈 뼈대**예요(prd.md 채우고 AI로 만들면 진짜 화면이 나와요):
  - 브라우저로 더블클릭해서 열기, 또는
  - **Live Server**: 파일 우클릭 → **Open with Live Server** (또는 우측 하단 **Go Live**)
  - 마크다운(`.md`) 미리보기: **Ctrl+Shift+V**

### ③ 내 것으로 바꾸기 (OpenCode)
- `prd.md`를 내 기획으로 채우기
- OpenCode에 **하나씩** 부탁 → 저장 → 브라우저에서 확인 → 다시 부탁
- 멈추기 전 `context.md`의 "다음에 할 일" 갱신

## 5. 배포하기 (내 저장소 → GitHub Pages)
> 수업 저장소(AightLabs/...)는 함께 쓰는 것이라 **직접 올릴 수 없어요.** 반드시 **내 저장소**를 새로 만들어 올립니다.
1. VS Code에서 내 폴더 열기 → **Source Control** (왼쪽 가지 아이콘)
2. 메시지 `first commit` → **✓ Commit**
3. **Publish to GitHub → public** 선택 → 내 저장소가 생성됨
4. GitHub 저장소 → **Settings → Pages → Branch: `main` /(root) → Save**
5. 1~2분 뒤 공개 주소: `https://내아이디.github.io/내저장소/`

## 6. 자주 막히는 곳
- **만들었는데 게임/화면이 안 나와요** → 브라우저 콘솔(F12)의 빨간 에러를 복사해 OpenCode에게 주기 (Phaser·Tailwind는 CDN이라 인터넷 연결도 확인)
- **배포 404** → 파일명이 `index.html`인지, Pages Branch가 `main`인지, 1~2분 기다렸는지
- **바꿨는데 사이트에 반영 안 됨** → `Commit` 후 `Push(Sync)` 했는지 확인 → 강력 새로고침(Ctrl+Shift+R)
- **모델이 느리거나 막힘** → OpenCode에서 `/models`로 다른 무료 모델 전환

---
문의·수정은 저장소 이슈로: https://github.com/AightLabs/jdh-school-vibe-coding
