## セッション管理の改善

`/new`や`/clear`コマンドで新しいセッションに名前を付けられるようになった。重要なスレッドのピン留めや、サイドスレッド間の切り替えも可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## Agent Pluginsサポートの追加

Agent Pluginsマニフェストのサポート、ワークスペースプラグイン公開機能、Amazon BedrockおよびClaude Code向けのマーケットプレイス連携が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## スレッドフォーク機能の実装

ページネーション付きのスレッド履歴フォークが実装された。標準のスレッド一覧に表示されない一時フォークもサポートされている。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## リモートCode ModeのWebSocket接続

WebSocketプロトコルを使用して、リモートCode Modeホストへのアプリサーバー接続が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## スタンドアロンWeb検索機能

カスタムモデルプロバイダーがスタンドアロンのWeb検索機能をオプトインできるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## Executor提供スキルの発見機能

Executor提供のスキル発見と、関連リソースへのセキュアなアクセスが実装された。明示的に選択されたスキルのリソース読み取りも含まれる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## プロキシ対応の包括的改善

認証、プラグインダウンロード、MCP認可、リモート実行、WebSocket、リダイレクト、LM Studio接続にわたるプロキシ設定が包括的に改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## MCP接続管理の改善

認証やコンフィギュレーション変更時にMCP接続が維持されるようになり、不必要な再起動が回避されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## メッセージ保持の強化

中断、リプレイ、インポート、フォーク時に送信済みメッセージ、最終レスポンス、承認設定が保持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## ターミナルレスポンシブネスの改善

ノンブロッキング割り込み、キーボードハンドリングの改善、狭いレイアウト対応、ハイパーリンクレンダリングによりTUIパフォーマンスが向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## Windowsおよびプロセス管理の修正

Windowsのナビゲーションキーの修正、サンドボックス化されたプロセスツリーの確実な終了、セキュリティレビュー時のプロキシ設定保持が改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## スキル保持の改善

コンテキスト予算が限られた場合のスキル保持が改善され、カタログの切り捨てが必要な場合は警告が表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## リリース配信インフラの移行

リリースアーティファクトの配信がOpenAIインフラに移行され、GitHubがフォールバックとして機能するようになった。macOSヘルパー実行ファイルの署名と公証も追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## シリアライゼーションの最適化

アプリサーバーのシリアライゼーションオーバーヘッド削減とリクエストビルドのメモリアロケーション最適化が行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)

## エンタープライズプラン認識と管理者更新制御

エンタープライズプランの認識機能と、管理者によるアプリ内更新制御が実装された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.146.0)
