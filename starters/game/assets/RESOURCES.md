# 🧰 게임용 리소스 (그래픽·효과음·음악)

> **두 종류예요:**
> - 📦 **이미 폴더에 든 것** — `images/`의 스프라이트 SVG는 바로 쓰면 돼요 (아래 목록).
> - 🔗 **링크로 받는 것** — 효과음·배경음악은 파일이 아니라 사이트 링크예요. 필요하면 받아서 `audio/`에 넣어요.
> ⚠️ 다운로드한 것의 **라이선스(출처 표기 필요 여부)**를 꼭 확인하세요.

## 📦 이미 든 스프라이트 (`images/` 폴더 · 바로 사용)
`<img src="assets/images/coin.svg">` 또는 Phaser `this.load.image('coin','assets/images/coin.svg')`.

| | | | | |
|---|---|---|---|---|
| player | enemy | coin | apple | heart |
| gem | key | mushroom | shield | cloud |
| platform | bullet | star | basket | bomb |

> 총 15개. 더 필요하면 아래 사이트에서 받아 `images/`에 추가하세요.

## 🎨 그래픽 더 받기 (스프라이트·타일·UI)
| 이름 | 링크 | 라이선스 |
|---|---|---|
| **Kenney** ⭐ | kenney.nl/assets | **CC0**(표기 불필요) |
| **OpenGameArt** | opengameart.org | CC0/CC-BY 등(개별 확인) |
| **itch.io 무료 에셋** | itch.io/game-assets/free | 개별 확인 |
| **Game-icons.net** | game-icons.net | CC-BY(SVG 아이콘) |
| **Piskel**(직접 도트 그리기) | piskelapp.com | 내가 만듦 |

## 🔊 효과음 (SFX)
| 이름 | 링크 | 라이선스 |
|---|---|---|
| **Kenney Audio** ⭐ | kenney.nl/assets (Audio) | **CC0** |
| **Freesound** | freesound.org | CC0/CC-BY(개별 확인) |
| **jsfxr**(직접 만들기) | sfxr.me | 내가 만듦(무료) |
| **Pixabay Sound** | pixabay.com/sound-effects | 무료 |

## 🎵 배경음악 (BGM)
| 이름 | 링크 | 라이선스 |
|---|---|---|
| **Pixabay Music** ⭐ | pixabay.com/music | 무료(표기 불필요) |
| **FreePD** | freepd.com | CC0 |
| **Incompetech** | incompetech.com | CC-BY(표기 필요) |
| **Bensound** | bensound.com | 무료(표기) |

## 💡 코드에서 쓰기 (Phaser 예시)
```js
this.load.image('star', 'assets/images/star.png');
this.load.audio('pickup', 'assets/audio/sfx/pickup.ogg');
this.load.audio('bgm',    'assets/audio/music/theme.mp3');
```
> `.ogg`·`.mp3`·`.wav` 다 돼요. 파일을 폴더에 넣고 경로만 맞추면 끝.
