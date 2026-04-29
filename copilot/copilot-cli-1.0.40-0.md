## ACP クライアントのカスタムエージェント切り替え

ACP クライアントがエージェント設定オプションを通じてカスタムエージェントの一覧表示と切り替えが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-0)

## 割り込み動作の改善

Ctrl+C およびダブル Esc でキューに入っているメッセージが一括ではなく1つずつ削除されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-0)

## スラッシュコマンドランキングの改善

スラッシュコマンドのサジェスションがファジーマッチよりもプレフィックスマッチを優先するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-0)

## プロンプトモード (-p) のセキュリティ強化

プロンプトモード（-p）でリポジトリフックとワークスペース MCP がオプトイン環境変数（`GITHUB_COPILOT_PROMPT_MODE_REPO_HOOKS`、`GITHUB_COPILOT_PROMPT_MODE_WORKSPACE_MCP`）の明示的な設定を必要とするようになり、セキュリティデフォルトが強化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-0)

## バグ修正

- 複数のサーバーが同じ URL で異なる静的 OAuth クライアント ID を使用している場合に MCP OAuth トークンキャッシュが正しく動作しない問題が修正された
- ドットやその他の無効な文字を含む MCP ツール名が適切にサニタイズされるようになった

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-0)
