# Toolbox Pro

ブラウザで本格的に使えるツールを集めたサイトです。HTML / CSS / JavaScript だけで動き、サーバーもビルドも要りません。`main` に push すると Cloudflare Workers(静的アセット)で公開されます。

## ツール

| ツール | 場所 |
| --- | --- |
| DJターンテーブル Pro | `tools/dj-turntable-pro/` |
| DJデッキ | `tools/dj-decks/` |
| 小説読み上げ | `tools/novel-reader/` |

## 始まり

2026-11-11 に [smartools](https://github.com/kougin-amamn/smartools)(bc99ce5)から写して始めました。

- DJターンテーブル Pro と DJデッキは、コンセプトが違うため smartools から移しました。それまでの変更の履歴は smartools にあります。
- 小説読み上げは 2026-11-14 に smartools(d8a5425)から移しました。
- 共通の部品(`common/`)、試験の仕組み(`tests/`)、整形の設定、文書(`docs/`)も smartools から写しました。これからは、このリポジトリで別に育てます。
- 文書には smartools の他のツールへの言及が残っています。手を入れる時に、Toolbox Pro に合わせて直します。

## 試験

```bash
node tests/core.js
node tests/smoke.js all
node tests/scenarios/dj-turntable-pro.js
node tests/scenarios/dj-decks.js
```
