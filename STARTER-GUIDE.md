# 🧰 스타터 준비 & 사용 가이드

이 문서 하나로 **스타터가 무엇인지, 무엇이 들어 있는지, 어떻게 시작하고 배포하는지**를 정리했어요.
(강의 슬라이드: https://aightlabs.github.io/jdh-school-vibe-coding/ · 저장소: https://github.com/AightLabs/jdh-school-vibe-coding)

---

## 1. 스타터란?
"처음부터 빈 화면"이 아니라, **이미 돌아가는 완성 코드**에서 시작하는 시작 세트예요.
바로 실행해 보고, Copilot에게 말하며 내 것으로 바꿔 나갑니다.

두 가지가 있어요:

| 스타터 | 만들 것 | 스택 | 폴더 |
|---|---|---|---|
| 🎮 게임 | 웹게임 (별 받기 등) | **Phaser 3** | `starters/game/` |
| 🌟 비게임 | 소개/서비스 페이지 | **Tailwind CSS + Vanilla JS** | `starters/nongame/` |

## 2. 스타터 폴더에 들어 있는 것 (공통)
| 파일 | 역할 |
|---|---|
| `index.html` | **완성된 스타터 코드** — 여기를 고쳐요 (HTML 단일 파일 웹앱) |
| `prd.md` | **기획 템플릿** — 무엇을 만들지 5항목으로 정리 |
| `context.md` | **기억 파일** — "다음에 할 일"을 적어두는 곳 (컨텍스트 관리) |
| `README.md` | 그 스타터 전용 사용법 |

> 공통 특징: **HTML 파일 하나로 된 웹앱** + **GitHub Pages 배포 파이프라인**(커밋 → 푸시 → Pages).

## 3. 준비물 (수업 전/중)
- **GitHub 계정** (사전 가입 완료)
- **VS Code** · **Git** 설치 (슬라이드 CH3 참고)
- **GitHub Copilot** — 학생(Student) 플랜 권장. 무료(Free)면 채팅 월 50회 제한
- (권장) VS Code 확장 **Live Server** — 결과를 바로 미리보기

## 4. 시작하기 — 3단계

### ① 내려받기 (둘 중 하나)
- **방법 A · ZIP (가장 쉬움):** 저장소에서 초록 **Code → Download ZIP** → 압축 풀기
- **방법 B · git clone:**
  ```
  git clone https://github.com/AightLabs/jdh-school-vibe-coding.git
  ```

### ② 내 폴더로 복사 후 열기
- `starters/game` 또는 `starters/nongame` 폴더를 **바탕화면의 새 폴더**(영어 이름, 예: `my-game`)로 복사
- VS Code에서 그 새 폴더를 **File → Open Folder**
- `index.html`을 실행/미리보기:
  - 브라우저로 더블클릭해서 열기, 또는
  - **Live Server**: 파일 우클릭 → **Open with Live Server** (또는 우측 하단 **Go Live**)
  - 마크다운(`.md`) 미리보기: **Ctrl+Shift+V**

### ③ 내 것으로 바꾸기 (Copilot)
- `prd.md`를 내 기획으로 채우기
- Copilot Chat에 **하나씩** 부탁 → 저장 → 브라우저에서 확인 → 다시 부탁
- 멈추기 전 `context.md`의 "다음에 할 일" 갱신

## 5. 배포하기 (내 저장소 → GitHub Pages)
> 수업 저장소(AightLabs/...)는 함께 쓰는 것이라 **직접 올릴 수 없어요.** 반드시 **내 저장소**를 새로 만들어 올립니다.
1. VS Code에서 내 폴더 열기 → **Source Control** (왼쪽 가지 아이콘)
2. 메시지 `first commit` → **✓ Commit**
3. **Publish to GitHub → public** 선택 → 내 저장소가 생성됨
4. GitHub 저장소 → **Settings → Pages → Branch: `main` /(root) → Save**
5. 1~2분 뒤 공개 주소: `https://내아이디.github.io/내저장소/`

## 6. 자주 막히는 곳
- **실행했는데 게임이 안 나와요** → 인터넷 연결 확인(Phaser·Tailwind는 CDN). 브라우저 콘솔(F12)의 빨간 에러를 복사해 Copilot에게 주기
- **배포 404** → 파일명이 `index.html`인지, Pages Branch가 `main`인지, 1~2분 기다렸는지
- **바꿨는데 사이트에 반영 안 됨** → `Commit` 후 `Push(Sync)` 했는지 확인 → 강력 새로고침(Ctrl+Shift+R)
- **Copilot 한도 초과** → Free 플랜(월 50회). Tab 자동완성 활용 / 학생 플랜 활성화

---
문의·수정은 저장소 이슈로: https://github.com/AightLabs/jdh-school-vibe-coding
