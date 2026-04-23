## TUI クイック推論コントロール

TUI に推論レベルのクイックコントロールが追加された。`Alt+,` で推論を減少、`Alt+.` で増加でき、モデルアップグレード時は古い設定を維持せずデフォルトにリセットされる。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.124.0)

## マルチ環境セッションサポート

app-server セッションが複数環境に対応し、ターンごとの環境・作業ディレクトリ選択が可能になった。マルチワークスペースおよびリモートセットアップに対応する。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.124.0)

## Amazon Bedrock のファーストクラスサポート

AWS SigV4 署名とクレデンシャルベース認証による OpenAI 互換プロバイダー向けの Amazon Bedrock サポートが正式に追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.124.0)

## リモートプラグインマーケットプレイスの閲覧

リモートプラグインマーケットプレイスの一覧表示と読み取りが直接可能になり、より大きな結果ページに対応した。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.124.0)

## フックの安定化

フックが安定版となり、`config.toml` と `requirements.toml` でインライン設定が可能になった。MCP ツール、`apply_patch`、Bash セッションの監視にも対応した。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.124.0)

## Fast サービスティアのデフォルト化

対象の ChatGPT プランで、明示的にオプトアウトしない限り Fast サービスティアがデフォルトになった。

[参考リンク](https://github.com/openai/codex/releases/tag/v0.124.0)

## バグ修正

- ChatGPT の HTTP バック認証フローでの Cloudflare Cookie が保持されるようになり、認証の断絶が解消された
- リモート app-server の信頼性が向上。WebSocket イベントが負荷時にドレインされ、シャットダウン時にリモートワーカーの終了が処理される
- `/permissions` の変更がサイドカンバセーション間で維持されるよう、パーミッションモードドリフトが修正された
- `wait_agent` がメールボックスにキューされた作業がある場合にタイムアウトせず即座に返るよう修正
- ローカル stdio MCP の相対コマンドのフォールバックパス解決が修正された
- 起動時に不明なフィーチャー要件が中断ではなく警告を出すように変更され、起動失敗が減少した

[参考リンク](https://github.com/openai/codex/releases/tag/v0.124.0)
