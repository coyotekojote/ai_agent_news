## app-server デーモンライフサイクル管理の追加

実験的な `codex-app-server-daemon` クレートが追加され、リモートマシン上の Codex app-server を SSH 経由で管理するための機械可読ライフサイクルコマンド（`start`、`restart`、`stop`、`version`、`bootstrap`）が提供されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.2)

## Bedrock Mantle クライアントエージェントヘッダーの追加

Amazon Bedrock プロバイダリクエストに安定したクライアントエージェント HTTP ヘッダー（`x-amzn-mantle-client-agent: codex`）が追加され、セーフティスタックによる識別が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.2)

## SQLite の破壊的バージョンバンプの廃止

バージョン更新時に SQLite データベースを削除するメカニズムが廃止された。正規ファイル名（`state_5.sqlite` および `logs_2.sqlite`）に統合され、後方互換性のためにグレースフルマイグレーションに依存するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.2)

## スキルウォッチャーの app-server 移動

スキルウォッチャーが app-server に移動された。また、ファイルウォッチャーがコアモジュールから分離された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.2)

## ロール認識プラグイン共有コンテキスト API の追加

ロールを認識するプラグイン共有コンテキスト API が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.2)
