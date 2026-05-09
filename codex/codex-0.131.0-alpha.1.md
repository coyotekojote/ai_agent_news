## apply_patch フリーフォームのデフォルト有効化

`apply_patch` のフリーフォームモードがデフォルトで有効化された。従来の関数スタイルの `apply_patch` は削除された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## TUI ステータスラインの改善

ステータスラインにブレンドトークン数が表示されるようになった。また、パーミッションと承認モードも TUI ステータスラインに表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## サービスティアスラッシュコマンドの汎用化

サービスティア関連のスラッシュコマンドが汎用化され、config TOML で文字列形式のサービスティアを指定できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## モデル一覧の更新

`models.json` が更新され、利用可能なモデルの一覧が最新化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## openai ライブラリツールのサポート

openai ライブラリツールがサポートされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## エグゼキュータレジストリのリモート環境サポート

エグゼキュータレジストリがリモート環境をサポートするようになった。`CODEX_HOME` から設定済み環境を読み込めるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## デスクトップアテステーションの要求

デスクトップアプリからのアテステーション要求が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## リモートエンロールメントでのインストール ID 使用

リモートエンロールメントでインストール ID が使用されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## app-server のデーモンセーフリスタート対応

app-server がデーモンセーフなリスタートハンドリングをサポートするようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## 環境プロバイダスナップショットのパスフリー化

環境プロバイダのスナップショットがパスフリーになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## exec-server 環境トランスポートタイムアウトの増加

exec-server の環境トランスポートタイムアウトが延長され、信頼性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## コネクタディレクトリキャッシュの活用

ディスカバラブルツールリストにキャッシュされたコネクタディレクトリが使用されるようになり、パフォーマンスが向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## レガシーフックとツールヘルパーの削除

レガシーの after-tool-use フックと `ToolName` 表示ヘルパーが削除された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## API ヘッダーのハイフン区切り対応

セッションおよびスレッドヘッダーがハイフン区切り形式で送信されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)

## Darwin サンドボックスポリシーの改善

macOS の Seatbelt ネットワークポリシーからユーザーキャッシュ書き込みが削除され、サンドボックスのセキュリティが強化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.1)
