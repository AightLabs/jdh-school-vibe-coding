# 🛠️ 당일 세팅 가이드 — OpenCode + Zen 무료 모델

> 이 문서는 **수업 당일 처음 세팅해야 하는 AI 코딩 도구** 안내입니다. (강사 준비 + 학생 실습)
> 강의 슬라이드: https://aightlabs.github.io/jdh-school-vibe-coding/ · 저장소: https://github.com/AightLabs/jdh-school-vibe-coding

**Ollama 없이 · Windows(HP Omen) · VS Code + OpenCode(터미널) + OpenCode Zen 무료 모델**

---

## 구성 요약
- **Ollama 안 씁니다.** 클라우드의 Zen 무료 모델을 쓰므로 PC에 모델을 내려받을 필요가 없어 설치가 훨씬 간단합니다.
- 흐름: **VS Code 설치 → OpenCode 설치 → 실행 → Zen 가입(Google/GitHub) → API 키 복사 → `/connect`로 Zen 연결 → `/models`로 모델 선택.**

---

## ⚠️ Windows 설치 주의 — curl은 "그냥은" 안 됩니다
`curl … | bash` 설치 스크립트는 **bash가 필요**해서 일반 Windows(CMD/PowerShell)에선 안 돌아갑니다.

| 방법 | Windows | 비고 |
|---|---|---|
| **Scoop** `scoop install opencode` | ✅ 추천 | Windows 네이티브 패키지 매니저, 제일 깔끔 |
| **npm** `npm i -g opencode-ai` | ✅ | Node.js(v16+) 필요 |
| **Chocolatey** `choco install opencode` | ✅ | Windows 패키지 매니저 |
| curl `... \| bash` | △ | WSL 또는 Git Bash 안에서만 |
| bun | ✕ | Windows 지원 아직 진행 중 |
| brew | ✕ | macOS/Linux 전용 |
| paru | ✕ | Arch Linux 전용 |

> OpenCode는 공식적으로 Windows에서 "최고의 경험은 WSL"을 권장하지만, WSL은 리눅스 계층을 얹는 셋업이라 입문 수업엔 과합니다. **Scoop 또는 npm 네이티브 설치로 충분**하고, 문제가 생기면 그때 WSL을 고려하세요.

---

## 1단계. VS Code 설치
https://code.visualstudio.com 에서 다운로드 후 설치.

## 2단계. Node.js + OpenCode 설치 (npm 방식 · 이번 수업 채택)

OpenCode를 **npm**으로 설치합니다. npm은 **Node.js**에 딸려 오므로 Node.js를 먼저 깝니다.

**① Node.js 설치 (PowerShell)**
```powershell
winget install OpenJS.NodeJS.LTS
```
> winget이 안 되면 https://nodejs.org 에서 **LTS**를 받아 설치. 설치 후 **PowerShell을 껐다 켜세요**(경로 인식).

**② OpenCode 설치**
```bat
npm i -g opencode-ai
```

**③ 설치 확인**
```bat
node --version
opencode --version
```

**다른 방법(선택)** — Scoop `scoop install opencode` · Chocolatey `choco install opencode` (curl \| bash·bun·brew는 일반 Windows에서 안 됨)

## 3단계. OpenCode 실행
VS Code로 작업 폴더를 열고, VS Code **통합 터미널**(또는 일반 터미널)에서:
```bat
opencode
```

## 4단계. OpenCode Zen 가입 + API 키 복사
1. OpenCode Zen 웹 콘솔에서 **Google 또는 GitHub 로그인**으로 가입
2. API 키를 발급받아 **복사**
3. **결제수단(카드)은 등록하지 마세요.** 무료 모델은 카드 없이 되고, 등록 안 하면 실수로 유료 모델을 골라도 과금 대신 에러가 납니다(과금 위험 0)

## 5단계. `/connect`로 Zen 연결
OpenCode 안에서:
```
/connect
```
목록에서 **OpenCode Zen** 선택 → 복사한 API 키 붙여넣기.

## 6단계. `/models`로 모델 선택
```
/models
```
무료 모델 중 하나 선택. **기본값은 North Mini Code 추천**(이유는 아래 비교표).

---

## 7단계. 실제 사용법
작업 폴더 안에서 `opencode` 실행 후 자연어로 지시:
> 간단한 할 일 목록 웹앱을 HTML/JS 한 파일로 만들어줘.

**자주 쓰는 명령 / 단축키**
- `/models` — 모델 전환
- `Tab` — plan(계획) / build(실행) 모드 토글
- `@` — 프로젝트 파일 검색·참조
- `/undo`, `/redo` — 되돌리기 / 다시
- `/init` — 프로젝트에 `AGENTS.md` 생성
- `/help` — 전체 명령

**수업 전 테스트 프롬프트** (모델이 실제로 파일을 만드는지 확인)
> 웹 검색 없이, 순수 HTML/CSS/JS 한 파일로 간단한 메모 앱을 만들어줘. 메모 추가·목록·삭제·localStorage 저장까지. 코드를 파일로 작성해줘.

---

## 무료 모델 비교 (코딩 기준)

| 모델 | 정체 | 코딩·에이전트 | 속도 | 이 수업엔 |
|---|---|---|---|---|
| **North Mini Code** | Cohere 첫 코딩 전용 모델 | **OpenCode 도구에 맞춰 튜닝**(tool calling 신뢰도 최상), 크기 대비 코딩 최상위 | 매우 빠름 | ★ 1순위(기본값) |
| **DeepSeek V4 Flash** | DeepSeek 빠른 코더 | 원 코딩 품질 살짝 위(더 큰 모델), 에이전트 견고 | 빠름 | 어려운 과제용 2순위 |
| **Big Pickle** | 사실상 GLM-4.6(Zhipu) | 준수한 올라운더 + 200k 컨텍스트, tool calling은 상위권만큼은 아님 | 보통 | 긴 컨텍스트 필요 시 |
| **MiMo V2.5** | Xiaomi 코딩 모델 | 무난한 코딩 특화, 중위권 | 빠른 편 | 무난한 대안 |
| **Nemotron 3 Ultra** | NVIDIA 대형 범용 | 코딩 특화 아님, "trial 전용", 느림 | 느린 편 | 이 용도엔 비추 |

**추천 운영**
- 기본값 **North Mini Code** — OpenCode 전용 튜닝 + 최고 속도라 "말로 시키면 파일을 만들고 고치는" 동작이 가장 안정적. 입문 바이브코딩에 최적.
- 무거운 로직/디버깅만 **DeepSeek V4 Flash**로 전환, 큰 프로젝트는 **Big Pickle**.
- **Nemotron 3 Ultra는 빼세요**(범용 대형·trial 전용·느림).

---

## 🔒 데이터 안전 규칙 (미성년자 수업 필수)
무료 기간엔 이 모델들의 입력이 모델 개선에 쓰일 수 있고, 특히 **North Mini Code·Nemotron은 "개인·기밀 정보 입력 금지"**라고 명시돼 있습니다. 학생들에게 **코딩 과제만 입력, 이름·연락처 등 개인정보는 절대 넣지 않기**를 규칙으로 정하세요.

## ⚠️ 수업 안정성 주의
Zen 무료 모델은 ① **"for a limited time"**이라 수업 직전·도중에 사라질 수 있고, ② **10명 동시 사용 시 속도 제한**에 걸릴 수 있습니다. **수업 하루 전 반드시 리허설**로 확인하고, 막히면 유료 모델(소액 충전)로 전환하거나 로컬 모델(Ollama) 대안을 다시 꺼낼 수 있게 대비해 두세요.

## 🖥️ 10대 배포 팁
- 1대에서 전체 흐름(설치 → 가입 → 연결 → 모델선택 → 테스트 프롬프트)을 검증한 뒤 나머지 PC에 동일 반복.
- **Zen 키 전략:** 학생별로 각자 가입해 개별 키를 쓰면 계정별 한도를 각자 받아 동시 사용 시 throttle에 덜 걸립니다. 대신 미성년자 가입(구글/깃허브 계정 + Zen)은 학교/보호자 정책을 확인하세요. 하나의 키를 10대가 공유하면 세팅은 간단하지만 동시 사용 시 제한에 더 잘 걸립니다.
- "기본은 무료 모델, 유료 전환은 강사 확인 후"를 규칙으로 정하면 비용이 안정적입니다.

---

## 체크리스트 (당일 아침)
- [ ] VS Code 설치 확인
- [ ] OpenCode 설치 (`opencode --version`)
- [ ] Zen 가입 + API 키 (카드 미등록)
- [ ] `/connect` → Zen 연결
- [ ] `/models` → North Mini Code 선택
- [ ] 테스트 프롬프트로 파일 생성 확인
- [ ] (강사) 리허설 1회 · 백업 계획(유료 소액/Ollama)
- [ ] 학생 규칙 공지: **개인정보 입력 금지**
