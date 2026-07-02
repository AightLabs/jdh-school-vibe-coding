# 🌟 비게임 웹앱 스타터 (Tailwind + Vanilla JS)

깔끔한 **자기소개 페이지**가 이미 완성되어 있어요. 응원 버튼·다크모드 같은 동작 예시도 들어 있어요.

## 스택
- **Tailwind CSS** (클래스로 꾸미는 도구, CDN으로 불러옴 → 인터넷 필요)
- **Vanilla JS** (순수 자바스크립트, 라이브러리 없음)
- HTML 파일 **하나**로 된 웹앱 → GitHub Pages로 그대로 배포 가능

## 폴더에 든 것
| 파일 | 설명 |
|---|---|
| `index.html` | 완성된 소개 페이지 (여기를 고쳐요) |
| `prd.md` | 웹앱 기획서 템플릿 |
| `context.md` | 프로젝트 기억 파일 (다음에 할 일 메모) |

## 1) 열어서 실행 · 미리보기
- `index.html`을 **브라우저로 더블클릭**해서 열면 바로 보여요.
- VS Code에서는 확장 **Live Server** 설치 후 **Go Live** (또는 파일 우클릭 → Open with Live Server).
- `prd.md` 같은 마크다운은 VS Code에서 **Ctrl+Shift+V**로 미리보기.

## 2) 내 페이지로 꾸미기
- **꾸미기(색·크기·배치):** 태그의 `class="..."` 안 Tailwind 클래스 (예: `bg-indigo-600` → `bg-emerald-600`)
- **움직임(버튼 동작):** 파일 맨 아래 `<script>` 안 자바스크립트
- OpenCode 예시:
```
지금 이 index.html은 Tailwind로 만든 소개 페이지야. prd.md를 참고해서
제목을 내 이름으로, 좋아하는 것 3가지를 실제 내용으로, 색을 초록 계열로 바꿔줘.
초보용 한국어 주석을 달고 전체 코드를 보여줘.
```

## 3) 내 저장소로 배포하기 (GitHub Pages)
> 수업 저장소는 함께 쓰는 것이라 바로 올릴 수 없어요. **내 폴더로 복사**한 뒤 **내 저장소**를 만들어 올려요.
1. 이 `nongame` 폴더를 **바탕화면의 새 폴더**(영어 이름)로 복사.
2. VS Code에서 그 새 폴더를 **Open Folder**.
3. **Source Control → Commit → Publish to GitHub → public**.
4. GitHub **Settings → Pages → Branch: main /(root) → Save**.
5. 1~2분 뒤 `https://내아이디.github.io/내저장소/` 에서 공개!
