## Vim ビジュアルモードの追加

Vim のビジュアルモード（`v`）およびビジュアルラインモード（`V`）が追加された。選択、オペレーター、ビジュアルフィードバックに対応している。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/cost` と `/stats` の統合

`/cost` と `/stats` が `/usage` に統合された。両コマンドは引き続きタイピングショートカットとして使用でき、関連タブが開かれる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## カスタムテーマ機能

`/theme` から名前付きカスタムテーマを作成・切り替えできるようになった。`~/.claude/themes/` の JSON ファイルを直接編集でき、プラグインも `themes/` ディレクトリ経由でテーマを配布可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フックからの MCP ツール直接呼び出し

フックで `type: "mcp_tool"` を指定することで MCP ツールを直接呼び出せるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `DISABLE_UPDATES` 環境変数の追加

`DISABLE_UPDATES` 環境変数が追加され、手動の `claude update` を含むすべての更新パスを完全にブロックできるようになった。`DISABLE_AUTOUPDATER` よりも厳格な制御が可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WSL での Windows マネージド設定の継承

WSL on Windows で `wslInheritsWindowsSettings` ポリシーキーにより、Windows 側のマネージド設定を継承できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## オートモードの `$defaults` サポート

`autoMode.allow`、`autoMode.soft_deny`、`autoMode.environment` に `"$defaults"` を含めることで、ビルトインリストを置き換えずにカスタムルールを追加できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## オートモードオプトインの「再度確認しない」オプション

オートモードオプトインプロンプトに「Don't ask again」オプションが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude plugin tag` コマンドの追加

プラグインのバージョン検証付きリリース Git タグを作成する `claude plugin tag` コマンドが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `--continue`/`--resume` の改善

`/add-dir` で現在のディレクトリを追加したセッションも `--continue`/`--resume` で検出されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/color` の Remote Control 同期

Remote Control 接続時に `/color` でセッションのアクセントカラーが claude.ai/code に同期されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/model` ピッカーのカスタムゲートウェイ対応

カスタム `ANTHROPIC_BASE_URL` ゲートウェイ使用時に `/model` ピッカーが `ANTHROPIC_DEFAULT_*_MODEL_NAME`/`_DESCRIPTION` オーバーライドを反映するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグイン自動更新スキップの通知

バージョン制約により自動更新がスキップされたプラグインが `/doctor` と `/plugin` の Errors タブに表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

- `/mcp` メニューで `headersHelper` 設定済みサーバーの OAuth 認証/再認証アクションが非表示になる問題を修正
- カスタムヘッダー付き HTTP/SSE MCP サーバーが一時的な 401 後に「needs authentication」のまま停止する問題を修正
- OAuth トークンレスポンスに `expires_in` が含まれない MCP サーバーで毎時再認証が必要になる問題を修正
- MCP ステップアップ認可で、サーバーの `insufficient_scope` 403 が現在のトークンに既にあるスコープを指定した場合にプロンプトなしでサイレントリフレッシュされる問題を修正
- MCP サーバーの OAuth フローがタイムアウトまたはキャンセルされた際の未処理 Promise リジェクションを修正
- MCP OAuth リフレッシュがプロセス間ロック競合時にロックなしで進行する問題を修正
- macOS キーチェーンレースで並行 MCP トークンリフレッシュが新しいトークンを上書きし「Please run /login」プロンプトが表示される問題を修正
- サーバーがローカル有効期限前にトークンを失効させた場合に OAuth トークンリフレッシュが失敗する問題を修正
- Linux/Windows で `~/.claude/.credentials.json` を破損させるクレデンシャル保存クラッシュを修正
- `CLAUDE_CODE_OAUTH_TOKEN` で起動したセッションで `/login` が無効だった問題を修正。環境トークンがクリアされディスククレデンシャルが有効になるようになった
- 「new messages」スクロールピルと `/plugin` バッジのテキストが読めない問題を修正
- `--dangerously-skip-permissions` 実行時にプラン承認ダイアログが「bypass permissions」ではなく「auto mode」を表示する問題を修正
- `Stop` / `SubagentStop` 以外のイベントに設定された agent-type フックが「Messages are required for agent hooks」で失敗する問題を修正
- `prompt` フックが agent-hook 検証サブエージェントによるツール呼び出しで再発火する問題を修正
- `/fork` がフォークごとに完全な親会話をディスクに書き込む問題を修正。ポインタを書き込み読み取り時にハイドレートするようになった
- `Alt+K` / `Alt+X` / `Alt+^` / `Alt+_` でキーボード入力がフリーズする問題を修正
- リモートセッションへの接続でローカルの `model` 設定が `~/.claude/settings.json` で上書きされる問題を修正
- `/` で始まるファイルパスを貼り付けた際に先行入力が「No commands match」エラーを表示する問題を修正
- 既にインストール済みのプラグインで `plugin install` が誤ったバージョンの依存関係を再解決しない問題を修正
- 無効なパスや fd 枯渇時のファイルウォッチャーからの未処理エラーを修正
- JWT リフレッシュ中の一時的な CCR 初期化ブリップで Remote Control セッションがアーカイブされる問題を修正
- `SendMessage` で再開されたサブエージェントが、スポーン時に指定された明示的な `cwd` を復元しない問題を修正

[参考リンク](https://code.claude.com/docs/en/changelog)
