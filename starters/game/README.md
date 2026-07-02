# 🎮 게임 스타터 (Phaser 3)

떨어지는 별을 받는 간단한 웹게임이 **이미 완성**되어 있어요. 여기서부터 내 게임으로 키워 보세요.

## 스택
- **Phaser 3** (게임 엔진, 인터넷 CDN으로 불러옴 → 실행하려면 인터넷 필요)
- HTML 파일 **하나**로 된 웹앱 → GitHub Pages로 그대로 배포 가능

## 폴더에 든 것
| 파일 | 설명 |
|---|---|
| `index.html` | 완성된 별 받기 게임 (여기를 고쳐요) |
| `prd.md` | 게임 기획서 템플릿 (내 게임을 정의) |
| `context.md` | 프로젝트 기억 파일 (다음에 할 일 메모) |

## 1) 열어서 실행 · 미리보기
- `index.html`을 **브라우저로 더블클릭**해서 열면 바로 실행돼요.
- VS Code에서는 확장 **Live Server** 설치 후, 파일을 우클릭 → **Open with Live Server** (또는 우측 하단 **Go Live**). 저장할 때마다 자동 새로고침돼요.
- `prd.md` 같은 마크다운은 VS Code에서 **Ctrl+Shift+V**로 미리보기.

## 2) 내 게임으로 바꾸기
1. `prd.md`를 열어 내 게임 기획을 채워요.
2. OpenCode에게 **하나씩** 부탁해요.
```
지금 이 index.html은 별 받기 게임이야. prd.md를 참고해서
(예: 빨간 폭탄을 추가하고 닿으면 게임오버) 를 만들어줘.
초보용 한국어 주석을 달고, 바뀐 전체 코드를 보여줘.
```
3. 멈추기 전 `context.md`의 "다음에 할 일"을 갱신해요.

## 3) 내 저장소로 배포하기 (GitHub Pages)
> 수업 저장소는 함께 쓰는 것이라 여기에 바로 올릴 수 없어요. **내 폴더로 복사**한 뒤 **내 저장소**를 만들어 올려요.
1. 이 `game` 폴더를 **바탕화면의 새 폴더**(영어 이름)로 복사해요.
2. VS Code에서 그 새 폴더를 **Open Folder**.
3. **Source Control → Commit → Publish to GitHub → public** 선택 (내 저장소가 생겨요).
4. GitHub 저장소 **Settings → Pages → Branch: main /(root) → Save**.
5. 1~2분 뒤 `https://내아이디.github.io/내저장소/` 에서 전 세계가 플레이!

> Phaser 버전을 올리려면 `index.html` 상단의 `phaser@3.80.1` 숫자를 바꾸면 돼요. (안정성 때문에 3 버전 권장)
