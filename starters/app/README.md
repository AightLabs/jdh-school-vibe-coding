# 🌟 앱 스타터 (빈 뼈대)

**아직 페이지가 없어요.** `prd.md`에 내 앱을 기획하고, AI(OpenCode)와 함께 만들어 나가는 **시작점**이에요.

## 폴더에 든 것
| 파일 | 설명 |
|---|---|
| `AGENTS.md` | **AI(OpenCode)가 자동으로 읽는 프로젝트 안내·규칙** |
| `prd.md` | **웹앱 기획서** — 뼈대 + 채운 예시. 여기부터 채워요 |
| `design.md` | 🎨 색·폰트·스타일 가이드 (AI가 읽음) |
| `context.md` | 프로젝트 기억 (다음에 할 일 메모) |
| `index.html` | **빈 뼈대** — 여기에 앱이 만들어져요 |
| `assets/` | 아이콘(SVG) 등 · `RESOURCES.md`(무료 출처) |

## 만드는 순서
1. **기획** — `prd.md`를 내 앱으로 채워요. (최소한만 채워도 OK · 미리보기 `Ctrl+Shift+V`)
2. **AI와 다듬기** — OpenCode에 검토를 받아요:
   ```
   이 폴더의 prd.md를 검토해줘. 빠진 항목이나 더 구체화할 부분,
   넣으면 좋을 기능을 나에게 하나씩 질문해줘.
   ```
   질문에 답하며 채우면 기획이 탄탄해져요.
3. **만들기** — 어느 정도 됐으면:
   ```
   이 폴더의 prd.md를 참고해서 index.html을 HTML/CSS/JS로 만들어줘.
   초보용 한국어 주석을 달아줘.
   ```
   저장 → Live Server로 확인 → **하나씩** 고쳐 부탁 (화면 뼈대 → 버튼 동작 → 색·꾸미기).
4. **이어가기** — 멈추기 전 `context.md`의 "다음에 할 일"을 갱신.

## 배포 (GitHub Pages)
> 수업 저장소는 함께 쓰는 것이라 바로 못 올려요. **내 폴더로 복사** → 내 저장소로.
1. 이 `app` 폴더를 **바탕화면의 새 폴더**(영어 이름)로 복사 → VS Code로 **Open Folder**
2. **Source Control → Commit → Publish to GitHub → public**
3. GitHub **Settings → Pages → Branch: main /(root) → Save**
4. 1~2분 뒤 `https://내아이디.github.io/내저장소/` 에서 공개!

> 💡 Tailwind CSS로 빠르게 꾸미려면 `index.html` 상단의 주석 처리된 Tailwind `<script>` 줄의 주석을 풀어요.
