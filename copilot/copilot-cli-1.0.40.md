## PR ブランチデコレーションの表示修正

PR ブランチのデコレーションがモデル名の長さに関わらず正しく表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## アシスタント応答のストリーミング改善

アシスタントの応答がよりスムーズなテキスト出力でストリーミングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## CLI 起動速度の改善

非同期の証明書読み込みにより CLI の起動速度が改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## /clear と /new でカスタムエージェント選択をリセット

`/clear` と `/new` がアクティブなカスタムエージェント選択をリセットするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## Azure DevOps リポジトリの自動検出

Azure DevOps リポジトリが検出された際に GitHub MCP サーバーが自動的に無効化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## MCP ツール名の特殊文字サニタイズ

特殊文字を含む MCP ツール名が適切にサニタイズされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## スキルのスラッシュコマンド化

スキルが ACP クライアントでスラッシュコマンドとして利用可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## セッション履歴と /chronicle コマンドの一般提供

セッション履歴と `/chronicle` コマンドが全ユーザーに提供されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## スラッシュコマンド提案の改善

スラッシュコマンドの提案ロジックが改善され、ランキングが強化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## プロンプトモードのセキュリティ強化

プロンプトモードでリポジトリフックとワークスペース MCP がオプトイン環境変数の指定を必要とするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)

## バグ修正

- /ask 応答ダイアログが開いている間もマウス選択が有効になった
- セッション切り替え時に保留中のメッセージが引き継がれなくなった
- セッション再開が誤って使用中と報告しなくなった

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40)
