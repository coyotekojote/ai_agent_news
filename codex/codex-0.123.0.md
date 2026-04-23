## Amazon Bedrock モデルプロバイダーの組み込み

AWS プロファイル設定に対応したビルトイン `amazon-bedrock` モデルプロバイダーが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.123.0)

## `/mcp verbose` コマンドの追加

`/mcp verbose` コマンドで詳細な診断情報が提供されるようになった。通常の `/mcp` は高速なまま維持される。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.123.0)

## プラグイン MCP ロードの拡張

プラグインの MCP ロードが `.mcp.json` 内の `mcpServers` とトップレベルサーバーマップの両方を受け入れるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.123.0)

## Realtime ハンドオフの改善

バックグラウンドエージェントがトランスクリプトデルタを受信し、明示的にサイレント状態を維持できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.123.0)

## ホスト固有のリモートサンドボックス設定

リモート環境向けの `remote_sandbox_config` 要件が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.123.0)

## バンドルモデルメタデータの更新

バンドルされたモデルメタデータが更新され、`gpt-5.4` がデフォルトとして設定された。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.123.0)

## バグ修正

- ロールバック後の `/copy` が、ロールバック前のレスポンスではなく最新の可視アシスタントレスポンスをコピーするよう修正
- 手動シェルコマンド実行中にキューされたフォローアップテキストがスタックする問題を修正
- VS Code WSL ターミナルでの Unicode/デッドキー入力が修正された（拡張キーボードモードの無効化）
- シェルスナップショットから古いプロキシ環境変数が復元されなくなった
- `codex exec` がサンドボックスやモデルオプションなどのルートレベルフラグを継承するよう修正
- TUI トランスクリプトからレビュープロンプトのリークが削除された

[参考リンク](https://github.com/openai/codex/releases/tag/v0.123.0)
