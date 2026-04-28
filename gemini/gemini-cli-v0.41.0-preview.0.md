## リアルタイムボイスモード

クラウドとローカルバックエンドの両方に対応したリアルタイムボイスモードが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/24174)

## 実験的 Gemma 4 モデルのサポート

実験的な Gemma 4 モデルバリアントのサポートが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25604)

## ContextManager と AgentChatHistory の接続

新しい ContextManager と AgentChatHistory が接続された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25409)

## 自動メモリスクラッチパッドの永続化

スキル抽出用の自動メモリスクラッチパッドが永続的に保存されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25873)

## settings.json の環境変数キャスト対応

settings.json の環境変数でブール値と数値のキャストがサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26118)

## セキュリティ強化

- `.env` ファイルのロードがセキュア化され、ヘッドレスモードでワークスペース信頼が強制されるようになった
- シェルコマンドの検証とコアツール許可リストが追加された
- YOLO モードでシェルパースが制限ルールに失敗した場合にフェイルクローズするようになった
- FatalUntrustedWorkspaceError にドキュメントリンクが追加された

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25814)

## 起動時間の改善

experiments と quota の読み込みが非同期で行われるようになり、起動時間が改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25758)

## UI・UX の改善

- ユーザーメッセージコンポーネントの背景色チェックが修正された
- 部分入力が空の場合のみ `list` サジェスションを表示するよう修正された
- Windows でのバックスペースハンドリングのリグレッションが修正された（リバート）
- ECONNRESET、ETIMEDOUT、ENOTDIR のエラーメッセージが改善された
- cloudshell-gca 認証失敗時のエラーメッセージがより分かりやすくなった

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-preview.0)

## CLI の改善

- コマンドの出力リダイレクトが対応された
- カスタムテーマテキストスキーマに不足していた `response` キーが追加された
- 自動アップデート失敗時に手動アップデートコマンドが表示されるようになった
- コマンドラインからのセッション UUID 手動指定が可能になった
- MCP の ping が list コマンドでオプションとなり、設定されたタイムアウトが使用されるようになった
- SessionEnd フックからの ACP stdout 汚染が防止された
- DevTools アクティビティロガーで Request ヘッダーが保持されるようになった

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-preview.0)

## インフラ・メンテナンス

- サンドボックスプロキシのクリーンアップとハンドラーリークが修正された
- 並列タスクトラッカー更新が強制されるようになった
- 一時的なエラーがターミナルとしてマークされないよう修正された
- 非文字列のモデルフラグが正しく処理されるようになった
- JetBrains IDE での代替バッファ警告ロジックが修正された
- gemini-cli-bot のメトリクスとワークフローが追加された
- 時系列メトリクス分析とリポジトリ管理提案のボットが実装された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-preview.0)

## ドキュメント・テスト

- README に Gemini CLI コースリンクが追加された
- サンドボックスのドキュメントが更新された
- ACP コマンドの復元に関するユニットテストが追加された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-preview.0)

## ループ検出時の致命的クラッシュ修正

ループ検出時の未処理 AbortError による致命的クラッシュが修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/20108)
