## Azure DevOps リポジトリの自動検出

Azure DevOps リポジトリが検出された場合に GitHub MCP サーバーが自動的に無効化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-1)

## セッション履歴・ファイル追跡・/chronicle コマンドの一般提供

セッション履歴、ファイル追跡、および `/chronicle` コマンドが全ユーザーに公開された（以前はゲート付き機能）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-1)

## ACP クライアントでのスキルスラッシュコマンド対応

スキルが ACP クライアントでスラッシュコマンドとして利用可能になり、CLI と同等の体験が提供されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-1)

## カスタム CA 証明書の非同期読み込みによる起動高速化

カスタム CA 証明書の読み込みが非同期化され、CLI の起動速度が向上した。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-1)

## リモートコントロールリンクの表示改善

リモートコントロールリンクがタイムラインに完全な URL で表示されるようになった（以前は「Open in browser」という汎用テキストだった）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-1)

## ACP クライアントでのライブプラン表示

ACP クライアント（例: Zed）で、エージェントがマルチステップタスクを処理する際のライブプランが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-1)

## ステータスラインピッカーのカスタムコマンド表示トグル

ステータスラインピッカーにカスタム `statusLine.command` の表示・非表示を切り替えるトグルが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-1)

## バグ修正

- 前回の CLI プロセスが予期せず終了した後にセッションを再開すると「使用中」と誤って報告される問題が修正された
- `--config-dir` がプラグインサブコマンドに正しく伝播されるようになった。`--config-dir` は `COPILOT_HOME` 環境変数に置き換えられ非推奨となった
- `/ask` レスポンスダイアログが開いている間もマウス選択が機能するようになった（以前はブロックされていた）

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-1)
