# 🌟 비게임 웹앱 스타터 (Tailwind + Vanilla JS)

깔끔한 **자기소개 페이지**가 이미 완성되어 있어요. 응원 버튼·다크모드 같은 동작 예시도 들어 있어요.

## 스택
- **Tailwind CSS** (클래스로 예쁘게 꾸미는 도구, CDN으로 불러옴 — 인터넷 필요)
- **Vanilla JS** (순수 자바스크립트, 라이브러리 없음)
- HTML 파일 **하나**로 된 웹앱 → GitHub Pages로 그대로 배포 가능

## 바로 시작하기
1. 이 폴더의 **`index.html`** 을 브라우저로 열면 페이지가 보여요.
   - VS Code 확장 **Live Server** 의 **Go Live** 를 쓰면 편해요.
2. **`prd.md`** 를 열어 내 내용을 채워요.
3. Copilot Chat에게 **하나씩** 부탁하며 꾸며요.

```
지금 이 index.html은 Tailwind로 만든 소개 페이지야.
prd.md를 참고해서 제목을 내 이름으로, 좋아하는 것 3가지를 실제 내용으로,
색을 초록 계열로 바꿔줘. 초보용 한국어 주석을 달고 전체 코드를 보여줘.
```

## 꾸미기·움직임을 어디서 고치나요?
- **꾸미기(색·크기·배치):** 태그의 `class="..."` 안 Tailwind 클래스 (예: `bg-indigo-600` → `bg-emerald-600`)
- **움직임(버튼 동작):** 파일 맨 아래 `<script>` 안 자바스크립트

## 내 프로젝트로 만들기 → 배포
1. `nongame` 폴더를 내 작업 폴더로 복사(또는 `index.html`·`prd.md`만 복사).
2. VS Code에서 **Source Control → Commit → Publish to GitHub (public)**.
3. GitHub 저장소 **Settings → Pages → Branch: main /(root) → Save**.
4. 1~2분 뒤 `https://내아이디.github.io/내저장소/` 에서 공개!

## 파일
| 파일 | 설명 |
|---|---|
| `index.html` | 완성된 소개 페이지 (여기를 고쳐요) |
| `prd.md` | 웹앱 기획서 템플릿 |
