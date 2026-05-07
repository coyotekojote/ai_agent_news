## TUI モーダル Vim 編集サポート

TUI コンポーザーでモーダル Vim 編集がサポートされた。`/vim` コマンド、デフォルトモード設定、Vim 固有のキーマップコンテキストが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## ワークフロー管理の改善

セッションの再開とコピーが容易になるよう、リデザインされたピッカーインターフェース、生のスクロールバックモード、`/ide` コンテキストインジェクション、ワークスペース対応の `/diff` 機能が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## ステータスラインの強化

ステータスラインがテーマ対応カラーとオプションの PR およびブランチ変更サマリーを表示できるようになった。`/keymap debug` でターミナルキーイベントの検査が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## プラグイン管理の拡張

プラグイン管理が大幅に強化され、ワークスペース共有、アクセス制御、ソースフィルタリング、ローカルパス追跡、マーケットプレイス操作、リモートバンドル同期、管理者ステータス処理が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## フックシステムの改善

`/hooks` コマンドでフックの閲覧と切り替えが可能になった。コンパクション前後のフック実行と `PreToolUse` コンテキストがサポートされた。Codex Apps 認証と対象の MCP エリシテーションが TUI/Guardian フローを通じて利用可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## 実験的ゴール機能

ゴール機能の発見性が向上し、ユーザーがオプトインしない限りリジューム時に一時停止状態が維持されるようになった。バリデーションと複数日期間表示も改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## 入力・クリップボードの修正

tmux 環境での `/copy` の動作が改善された。Alt+Enter および修正された Delete/Backspace キーの挙動が修正された。Windows でのタイピング/ペーストのレイテンシが削減された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## Linux サンドボックスの信頼性向上

古い bwrap バージョン、遅いマウントプローブ、シンボリックリンク保護パス、共有 `/tmp` 設定など、Linux サンドボックスのスタートアップ信頼性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## Windows サンドボックスと実行の改善

名前付きパイプ、ConPTY のティアダウン、PowerShell ラップされた許可ルール、ワークツリーの safe.directory、安全でない Git オプションの処理が強化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## セキュリティと設定の修正

TLS インスペクションプロキシ背後のカスタム CA ログイン、Bedrock ランタイムエンドポイントレポート、危険なプロジェクト設定キー、ヒアドキュメントリダイレクト承認マッチング、無制限の MCP/フック出力増加に関する問題が修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)

## インフラストラクチャ改善

npm および DotSlash インストール用にスタンドアロン `bwrap` フォールバックがバンドルされた。ベンダリングされた Bubblewrap が 0.11.2 にアップデートされ、上流のセキュリティ改善が含まれた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0)
