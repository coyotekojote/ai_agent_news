## フォーク型サブエージェントの外部ビルド対応

`CLAUDE_CODE_FORK_SUBAGENT=1` を設定することで、外部ビルドでもフォーク型サブエージェントを有効化できるようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## エージェントフロントマター `mcpServers` の読み込み

`--agent` によるメインスレッドエージェントセッションでも、エージェントフロントマターの `mcpServers` が読み込まれるようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## `/model` 選択の永続化改善

モデル選択がプロジェクト側で異なるモデルを指定していても再起動後に維持されるようになった。起動ヘッダーにアクティブなモデルがプロジェクトまたはマネージド設定のピンによるものかが表示される。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## `/resume` セッション要約

古く大きなセッションの再開時に、再読み込み前にセッションを要約するかどうか確認されるようになった。既存の `--resume` の動作と統一された。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## MCP 起動の高速化

ローカルと claude.ai の両方の MCP サーバーが設定されている場合、同時接続がデフォルトになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## `plugin install` の改善

既にインストール済みのプラグインに対して `plugin install` を実行すると、不足している依存関係がインストールされるようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## プラグイン依存関係のエラーメッセージ改善

プラグイン依存関係のエラーメッセージに「not installed」とインストールヒントが表示されるようになった。`claude plugin marketplace add` が設定済みマーケットプレイスから不足依存関係を自動解決する。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## マネージド設定の強制

`blockedMarketplaces` と `strictKnownMarketplaces` がプラグインのインストール、更新、リフレッシュ、自動更新時に強制されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## Advisor Tool（実験的機能）

ダイアログに「experimental」ラベル、詳細リンク、有効化時の起動通知が追加された。「Advisor tool result content could not be processed」エラーでセッションが停止する問題も修正された。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## `cleanupPeriodDays` 保持スイープの拡張

クリーンアップ対象に `~/.claude/tasks/`、`~/.claude/shell-snapshots/`、`~/.claude/backups/` が追加された。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## OpenTelemetry の強化

`user_prompt` イベントにスラッシュコマンド用の `command_name` と `command_source` が含まれるようになった。`cost.usage`、`token.usage`、`api_request`、`api_error` にモデルがエフォートレベルをサポートする場合 `effort` 属性が追加された。カスタム/MCP コマンド名は `OTEL_LOG_TOOL_DETAILS=1` を設定しない限り秘匿される。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## ネイティブビルドへの `bfs` と `ugrep` の組み込み

macOS と Linux のネイティブビルドで `Glob` と `Grep` ツールが組み込みの `bfs` と `ugrep` に置き換えられた。Bash ツール経由でより高速な検索が可能になった（Windows および npm インストールビルドは変更なし）。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## Windows パフォーマンス改善

`where.exe` による実行ファイルルックアップがプロセスごとにキャッシュされ、サブプロセスの起動が高速化された。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## デフォルトエフォートレベルの変更

Pro/Max サブスクライバーにおける Opus 4.6 および Sonnet 4.6 のデフォルトエフォートが `medium` から `high` に変更された。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## バグ修正

- Plain-CLI の OAuth セッションでアクセストークンがセッション中に期限切れになると「Please run /login」で停止する問題を修正。401 時にトークンが自動リフレッシュされるようになった
- 非常に大きな HTML ページで `WebFetch` がハングする問題を修正。HTML→Markdown 変換前に入力がトランケートされるようになった
- プロキシが HTTP 204 No Content を返した際にクラッシュする問題を修正。TypeError の代わりに明確なエラーが表示されるようになった
- `CLAUDE_CODE_OAUTH_TOKEN` 環境変数で起動しそのトークンが期限切れになった場合に `/login` が効果を持たない問題を修正
- `Ctrl+_` による入力のアンドゥが入力直後に動作しない問題と、各アンドゥステップで状態がスキップされる問題を修正
- Bun 実行時にリモート API リクエストで `NO_PROXY` が尊重されない問題を修正
- 低速接続でキー名がテキストとして結合された際にまれにエスケープ/リターンが誤発火する問題を修正
- SDK の `reload_plugins` がすべてのユーザー MCP サーバーをシリアルに再接続していた問題を修正
- Opus 4.7 の思考無効化時に Bedrock アプリケーション推論プロファイルリクエストが 400 で失敗する問題を修正
- print/SDK モードでサーバーがターン中に接続完了した際に `elicitation/create` リクエストが自動キャンセルされる問題を修正
- サブエージェントがメインエージェントと異なるモデルを実行している場合にファイル読み取りでマルウェア警告が誤表示される問題を修正
- バックグラウンドタスク存在時のアイドル再レンダリングループによる Linux でのメモリリークを修正
- 複数の大きなマーケットプレイスが設定されている場合に VS Code の「Manage Plugins」パネルが壊れる問題を修正
- Opus 4.7 セッションで `/context` パーセンテージが過大表示され、早期に自動コンパクトされる問題を修正。200K ではなく Opus 4.7 ネイティブの 1M コンテキストウィンドウで計算されるようになった

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
