## MCP サーバー設定に `alwaysLoad` オプション追加

`alwaysLoad` を `true` に設定すると、そのサーバーのすべてのツールがツール検索の遅延をスキップし、常に利用可能になる。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## `claude plugin prune` コマンド

孤立した自動インストール済みプラグイン依存を削除する `claude plugin prune` コマンドが追加された。`plugin uninstall --prune` でカスケード削除も可能。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## `/skills` のタイプ入力フィルター検索

`/skills` にタイプ入力によるフィルター検索ボックスが追加され、長いリストをスクロールせずにスキルを検索できるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## PostToolUse フックの出力置換が全ツールに拡張

`hookSpecificOutput.updatedToolOutput` による PostToolUse フックのツール出力置換が、従来の MCP 限定から全ツールに対応した。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## 非インタラクティブセッションでの `CLAUDE_CODE_FORK_SUBAGENT=1` 対応

`CLAUDE_CODE_FORK_SUBAGENT=1` が SDK や `claude -p` などの非インタラクティブセッションでも動作するようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## `/terminal-setup` での iTerm2 クリップボードアクセス有効化

`/terminal-setup` が iTerm2 の「Applications in terminal may access clipboard」を有効にし、tmux からの `/copy` も動作するようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## Vertex AI: X.509 証明書ベースの Workload Identity Federation (mTLS ADC) サポート

Vertex AI で X.509 証明書ベースの Workload Identity Federation（mTLS ADC）がサポートされた。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## SDK: `mcp_authenticate` の `redirectUri` サポート

SDK の `mcp_authenticate` がカスタムスキーム完了や claude.ai コネクタ用の `redirectUri` をサポートするようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## OpenTelemetry の強化

LLM リクエストスパンに `stop_reason`、`gen_ai.response.finish_reasons`、および `user_system_prompt`（`OTEL_LOG_USER_PROMPTS` でゲート）が追加された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## [VSCode] 音声ディクテーションの言語設定対応

Claude Code の言語設定が未設定の場合、音声ディクテーションが `accessibility.voice.speechLanguage` を参照するようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## [VSCode] `/context` がネイティブトークン使用量ダイアログを表示

VSCode で `/context` がネイティブのトークン使用量ダイアログを開くようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## フルスクリーンモードのスクロール修正

プロンプトへの入力時に、上方向にスクロールして過去の出力を読んでいた場合にスクロール位置が最下部に戻る問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## スクロール可能なオーバーフローダイアログ

ターミナルからはみ出すダイアログが矢印キー、PgUp/PgDn、Home/End、マウスホイールでスクロール可能になった（フルスクリーン・非フルスクリーン両対応）。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## 折り返し URL のクリック処理改善

フルスクリーンモードで複数行に折り返された長い URL のどの行をクリックしても完全な URL が開くようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## `--dangerously-skip-permissions` のスコープ拡張

`--dangerously-skip-permissions` 使用時に `.claude/skills/`、`.claude/agents/`、`.claude/commands/` への書き込みでプロンプトが表示されなくなった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## MCP サーバーの一時的エラー時の自動リトライ

MCP サーバーが起動時に一時的なエラーが発生した場合、接続不能のままにならず最大3回までリトライするようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## ターミナルタブのセッションタイトル

ターミナルタブのセッションタイトルが設定された `language` で生成されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## Claude.ai コネクタの重複排除

同じアップストリーム URL を持つコネクタが重複表示されず、重複排除されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## アップグレード後の起動高速化

リリースノートのスプラッシュから最近のアクティビティパネルが削除され、起動が高速化された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## LSP 診断サマリーの改善

LSP 診断サマリーがクリック/Ctrl+O で展開されるようになり、展開ヒントが表示されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## Bash ツールのファイルディスクリプタ使用量削減

大規模ディレクトリツリーでの `find` 実行時のピークファイルディスクリプタ使用量が削減された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)

## バグ修正

- 多数の画像を処理するセッションでの無制限メモリ増大（マルチGB RSS）が修正された
- 大規模なトランスクリプト履歴を持つマシンで `/usage` が最大約2GBのメモリリークを起こす問題が修正された
- 長時間実行ツールが進捗イベントをクリアに発行しない場合のメモリリークが修正された
- セッション開始ディレクトリが途中で削除・移動された場合に Bash ツールが永続的に使用不能になる問題が修正された
- 外部ビルドでの `--resume` 起動時クラッシュが修正された
- 不正シャットダウンによりトランスクリプト行が破損した場合の `--resume` 失敗が修正された（破損行はスキップされる）
- Bedrock アプリケーション推論プロファイル ARN 使用時の `thinking.type.enabled is not supported` エラーが修正された
- Microsoft 365 MCP OAuth で重複・非対応の `prompt` パラメータによる失敗が修正された
- tmux、GNOME Terminal、Windows Terminal、Konsole での非フルスクリーンモードで Ctrl+L や再描画時のスクロールバック重複が修正された
- 起動時の一時的な認証エラーで claude.ai MCP コネクタが無音で消える問題が修正された
- リモートセッションでのビルトインツールの「Always allow」ルールがワーカー再起動時に消える問題が修正された
- ネイティブビルドで `managed-settings.json` 経由で設定した `NO_PROXY` がすべての HTTP クライアントで尊重されない問題が修正された
- マネージド設定の承認プロンプトで承認しても終了してしまう問題が修正され、設定を適用して続行するようになった
- 古い OAuth トークンで `/usage` が「rate limited」を返す問題が修正され、自動リフレッシュされるようになった
- `settings.json` の無効なレガシー列挙値が設定ファイル全体を無効化する問題が修正された
- no-flicker モードがオフの場合に `/usage` ダイアログの内容が切れる問題が修正された
- フルスクリーンレンダラーがオフの場合に `/focus` が「Unknown command」と表示される問題が修正され、有効化方法が案内されるようになった
- 実行中のバイナリがセッション中に削除された場合に組み込みの grep/find/rg シェルラッパーが失敗する問題が修正され、インストール済みツールにフォールバックするようになった

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.121)
