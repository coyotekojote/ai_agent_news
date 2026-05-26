## ローカル会話履歴の検索機能

ローカルの会話履歴に対する検索機能が追加された。大文字・小文字を区別しない内容マッチングと結果プレビューが利用可能。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0)

## プロファイルセレクターの標準化

`--profile`がCLI、TUIパーミッション、サンドボックスフローにおけるプライマリプロファイル選択方法として統一され、レガシーなプロファイル設定が置き換えられた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0)

## MCPセットアップの強化

Model Context Protocolサーバーの設定が改善され、サーバーごとの環境ターゲティングやHTTPサーバーのOAuthサポートが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0)

## ツールスキーマの改善

コネクタツールスキーマがローカルの`$ref`/`$defs`構造を保持し、過大なスキーマを公開前にコンパクト化するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0)

## リードオンリーMCPツールの並行実行

`readOnlyHint`が付与されたリードオンリーMCPツールが並行して実行可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0)

## 拡張機能およびフックコンテキストの拡充

拡張ツールに会話履歴を含むリッチなコンテキストが追加され、フック入力にサブエージェントIDが含まれるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0)

## バグ修正・改善

WebSocketクライアントの再接続処理が改善され、古いexec-server接続に対する信頼性が向上した。リモートコントロールの認証リカバリ後のリトライロジックが改善された。リモートコンパクションv2ストリームにリトライロジックが追加された。Windows TUIの仮想ターミナルモード復元によりレンダリング破損が解消された。クレジットおよび利用上限エラー時にワークスペース固有のエラーメッセージが表示されるようになった。プラグインスキルが共有プラグインレベルのアイコンアセットを再利用可能になった。自動レビュー時のランタイム設定同期でアクティブなパーミッションプロファイルメタデータが保持されるようになった。Nodeベースツールがcodexのマネージドネットワークプロキシ環境を尊重するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0)
