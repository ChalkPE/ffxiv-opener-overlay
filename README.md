# ffxiv-opener-overlay

[ACT](https://advancedcombattracker.com/) [overlay](https://github.com/hibiyasleep/OverlayPlugin) for [Final Fantasy XIV](https://www.finalfantasyxiv.com/) that shows your real-time skill sequences.

![Summoner opener](public/smn-sb-opener.png)

* [In-game video (click to watch)](https://gaming.youtube.com/watch?v=sLJddcK1z6Y&feature=share)

## Installation

```url
https://chalkpe.github.io/ffxiv-opener-overlay
```

### OverlayPlugin

1. Open ACT
1. Plugins → OverlayPlugin.dll → New
1. Add new **Log Parse** type overlay (name is your choice)
1. Switch to the new overlay tab and set **URL** as above

### ACTWebSocket

1. Open ACT
1. Plugins → ACTWebSocket
1. Check **Using BeforeLogLineRead** on left panel
1. `Add URL` → set as above and select the new row → Click `Overlay`

## Requirements

### Client

| Language | Patch |
| :--: | :--: |
| 日本語 (`jp`) | `5.08` |
| English (`en`) | `5.08` |
| Deutsch (`de`) | `5.08` |
| Français (`fr`) | `5.08` |
| 한국어 (`kr`) | `4.5` |

### Configuration

* (`jp`) キャラクターコンフィグ → チャットログ設定 → ログフィルター設定 → バトル → `自分からのアクションの開始/中断`
* (`en`) Character Configuration → Log Window Settings → Log Filters → Battle → `Actions initiated by you.`
* (`de`) Configuration personnage → Fenêtre de log → Filtres du log → Combat → `Vos actions`
* (`fr`) Charakterkonfiguration → Chatlog → Chatfilter → Kampfhandlungen → `Eigenes Kommando`
* (`kr`) 캐릭터 설정 → 대화창 설정 → 로그 필터 설정 → 전투 → `자신의 기술 시작 및 중단`

## Usage

### Commands

* `/e toggle` - show/hide overlay
* `/e reset` - reset current sequence
* `/e scale <number>` - scale entire overlay (default: `1`)

## Development

### dev server

```bash
yarn && yarn serve
```

#### build & deploy

```bash
yarn && yarn build && yarn deploy
```

## License

[MIT License](LICENSE)

### /src/assets

```text
© 2010 - 2019 SQUARE ENIX CO., LTD. All Rights Reserved.
```
