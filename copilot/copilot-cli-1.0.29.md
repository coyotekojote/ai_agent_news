## Claude Opus 4.7 サポート

Claude Opus 4.7 モデルのサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.29)

## リモート MCP サーバー設定の簡略化

リモート MCP サーバー設定で `type` フィールドの省略が可能になり、デフォルトで `http` が適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.29)

## `--list-env` フラグの追加

プロンプトモードで読み込まれたプラグイン、エージェント、スキル、MCP サーバーを表示する `--list-env` フラグが追加され、CI/CD パイプラインでの環境検証が容易になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.29)

## セッション ID 環境変数

シェルコマンドと MCP サーバーが `COPILOT_AGENT_SESSION_ID` を環境変数として受け取るようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.29)

## バグ修正

- 点滅カーソルのアニメーション中にテキストがずれる問題が修正され、カーソル幅が安定するようになった
- リポジトリオーナーの識別がローカルシステムのユーザー名ではなく Git リモート URL から正しく行われるようになった
- Windows でクラッシュ終了後にターミナル状態が適切に復元されるようになった

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.29)
