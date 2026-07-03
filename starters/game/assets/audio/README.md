# 🔊 오디오 (효과음 · 음악)

여긴 **비어 있어요.** 소리 파일은 용량이 커서 미리 안 넣었어요 — 무료로 받아서 넣으세요.

- `sfx/`   : 효과음 (받기 `pickup.ogg`, 폭발 `boom.ogg` 등)
- `music/` : 배경음악 (`theme.mp3` 등)

## 어디서 받나 (무료)
- 효과음: **Kenney Audio**(CC0) · **Freesound** · **sfxr.me**(직접 생성)
- 음악:  **Pixabay Music** · **FreePD**(CC0)

자세한 링크·라이선스는 상위 폴더의 **`RESOURCES.md`** 를 보세요.

## 코드에서 (Phaser)
```js
this.load.audio('pickup', 'assets/audio/sfx/pickup.ogg');
this.load.audio('bgm',    'assets/audio/music/theme.mp3');
// ...
this.sound.play('pickup');
```
