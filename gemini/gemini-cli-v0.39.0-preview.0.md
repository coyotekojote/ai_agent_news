## サブエージェントの統合リファクタリング

サブエージェントツールが統一的な `invoke_subagent` 実装にリファクタリングされた。ツール呼び出しレコードにサブエージェントの永続的な `agentId` が記録されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)

## メモリとスキル管理

抽出されたスキルをレビューするための `/memory inbox` コマンドが追加された。メモリインボックスとの統合によるスキルパッチング機能もサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)

## ContextManager と Sidecar の分離

ContextManager と Sidecar のアーキテクチャが分離され、よりモジュラーな構成が実現した。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)

## プランモードの強化

- プランモードで `activate_skill` にユーザー確認が必要になった
- プランモードのモデルルーティングでサイレントフォールバックが追加された
- プラン内容の表示を許可するようプランモードプロンプトが更新された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)

## ストリーミングと記録

チャット記録が JSONL ストリーミング形式に移行された。`useAgentStream` フックが AppContainer に実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)

## メモリリーク修正

- リスナーのクリーンアップによるライフサイクルメモリリークの解消
- PTY 枯渇と孤立 MCP サブプロセスリークの防止
- 大容量出力ストリームでの OOM を防ぐバッファスライスの削除
- AbortSignal を使用した MessageBus でのサブエージェントメモリリークの修正

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)

## サンドボックスとセキュリティ

- すべてのプロセス実行パスで堅牢なサンドボックスクリーンアップが保証された
- Windows シンボリックリンクバイパスが解決された
- 読み取り専用制約付きの集中型非同期 Git worktree 解決が導入された
- ネイティブ ACL 適用による Windows サンドボックス初期化の最適化

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)

## UI の改善

- Windows Terminal で `Ctrl+Backspace` による単語削除がサポートされた
- AskUser 複数行回答でマウスクリックによるカーソル位置指定が可能になった
- スクロールモメンタムが強化された
- terminalBuffer モードでスクロールバーの表示が改善された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)

## パフォーマンス最適化

- 軽量な親プロセスによる起動の最適化
- メモリと CPU パフォーマンスの統合テストハーネスが追加された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.0)
