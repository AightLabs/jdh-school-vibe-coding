# 🎮 게임 스타터 (Phaser 3)

떨어지는 별을 받는 간단한 웹게임이 **이미 완성**되어 있어요. 여기서부터 내 게임으로 키워 보세요.

## 스택
- **Phaser 3** (게임 엔진, 인터넷에서 CDN으로 불러옴 — 실행하려면 인터넷 필요)
- HTML 파일 **하나**로 된 웹앱 → GitHub Pages로 그대로 배포 가능

## 바로 시작하기
1. 이 폴더의 **`index.html`** 을 브라우저로 열면 게임이 실행돼요.
   - VS Code에서 확장 **Live Server** 를 쓰면 더 편해요 (우측 하단 **Go Live**).
2. **`prd.md`** 를 열어 내 게임 기획을 채워요.
3. Copilot Chat에게 **하나씩** 부탁하며 키워요.

```
지금 이 index.html은 별 받기 게임이야.
prd.md를 참고해서 (예: 빨간 폭탄을 추가하고 닿으면 게임오버) 를 만들어줘.
초보용 한국어 주석을 달고, 바뀐 전체 코드를 보여줘.
```

## 내 프로젝트로 만들기 → 배포
1. `game` 폴더를 내 작업 폴더로 복사(또는 `index.html`·`prd.md`만 복사).
2. VS Code에서 **Source Control → Commit → Publish to GitHub (public)**.
3. GitHub 저장소 **Settings → Pages → Branch: main /(root) → Save**.
4. 1~2분 뒤 `https://내아이디.github.io/내저장소/` 에서 전 세계가 플레이!

## 파일
| 파일 | 설명 |
|---|---|
| `index.html` | 완성된 게임 (여기를 고쳐요) |
| `prd.md` | 게임 기획서 템플릿 |

> Phaser 버전을 올리고 싶으면 `index.html` 상단의 `phaser@3.80.1` 숫자를 바꾸면 돼요. (안정성 때문에 3 버전을 권장)
