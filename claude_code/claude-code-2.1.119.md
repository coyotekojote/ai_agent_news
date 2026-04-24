## `/config` 設定の永続化

`/config` の設定（テーマ、エディタモード、verbose 等）が `~/.claude/settings.json` に永続化されるようになり、プロジェクト/ローカル/ポリシーのオーバーライド優先順位にも参加するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `prUrlTemplate` 設定の追加

`prUrlTemplate` 設定が追加され、フッターの PR バッジを github.com ではなくカスタムコードレビュー URL に向けられるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `CLAUDE_CODE_HIDE_CWD` 環境変数

`CLAUDE_CODE_HIDE_CWD` 環境変数が追加され、起動ロゴの作業ディレクトリを非表示にできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `--from-pr` の対応プラットフォーム拡大

`--from-pr` が GitLab マージリクエスト、Bitbucket プルリクエスト、GitHub Enterprise の PR URL を受け付けるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `--print` モードのツール制御

`--print` モードがエージェントの `tools:` および `disallowedTools:` フロントマターに従うようになり、インタラクティブモードと同じ動作になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `--agent` のパーミッションモード対応

`--agent <name>` がビルトインエージェントのエージェント定義の `permissionMode` に従うようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PowerShell ツールコマンドの自動承認

パーミッションモードで PowerShell ツールコマンドが Bash と同様に自動承認できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェント・SDK MCP サーバーの並列接続

サブエージェントおよび SDK の MCP サーバー再設定時、サーバーが逐次ではなく並列で接続されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインのバージョン制約付き自動更新

別のプラグインのバージョン制約でピン留めされたプラグインが、満足する最高の git タグに自動更新されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vim モード: INSERT の Esc 動作改善

Vim モードで INSERT 中の Esc がキューされたメッセージを入力に引き戻さなくなった。中断するにはもう一度 Esc を押す必要がある。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スラッシュコマンドの表示改善

スラッシュコマンドサジェストでクエリに一致した文字がハイライトされるようになった。また、長い説明が切り詰められる代わりに2行目に折り返されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `owner/repo#N` ショートハンドリンクの改善

出力の `owner/repo#N` ショートハンドリンクが常に github.com を指すのではなく、git リモートのホストを使用するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フックの `duration_ms` 追加

`PostToolUse` および `PostToolUseFailure` フックの入力に `duration_ms`（パーミッションプロンプトや PreToolUse フックを除くツール実行時間）が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `blockedMarketplaces` の修正

`blockedMarketplaces` が `hostPattern` と `pathPattern` エントリを正しく適用するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OpenTelemetry の改善

`tool_result` および `tool_decision` イベントに `tool_use_id` が含まれるようになった。`tool_result` には `tool_input_size_bytes` も追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ステータスラインの改善

stdin JSON に `effort.level` と `thinking.enabled` が含まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

- CRLF コンテンツ（Windows クリップボード、Xcode コンソール）の貼り付けで行間に余分な空行が挿入される問題を修正
- kitty キーボードプロトコルシーケンスを使用するターミナルでの複数行貼り付けで改行が失われる問題を修正
- Bash ツールがパーミッションで拒否された際に macOS/Linux ネイティブビルドで Glob・Grep ツールが消える問題を修正
- フルスクリーンモードでスクロールアップ中にツール完了時に最下部にスナップバックする問題を修正
- MCP HTTP 接続で、サーバーが OAuth ディスカバリリクエストに非 JSON ボディを返した際に「Invalid OAuth error response」で失敗する問題を修正
- 画像添付付きメッセージで Rewind オーバーレイが「(no prompt)」を表示する問題を修正
- オートモードがプランモードを「Execute immediately」の指示で上書きする問題を修正
- レスポンスペイロードを出力しない非同期 `PostToolUse` フックがセッショントランスクリプトに空エントリを書き込む問題を修正
- サブエージェントのタスク通知がキューで孤立した際にスピナーが表示されたままになる問題を修正
- Vertex AI でサポートされていないベータヘッダーエラーを回避するためツール検索がデフォルトで無効化された（`ENABLE_TOOL_SEARCH` でオプトイン可能）
- スラッシュコマンド内で絶対パス付き `@` ファイルのタブ補完がプロンプト全体を置換する問題を修正
- macOS Terminal.app で Docker や SSH 経由で起動時にプロンプトに不正な `p` 文字が表示される問題を修正
- HTTP/SSE/WebSocket MCP サーバーの `headers` 内の `${ENV_VAR}` プレースホルダーがリクエスト前に置換されない問題を修正
- `--client-secret` で保存された MCP OAuth クライアントシークレットが `client_secret_post` を要求するサーバーでのトークン交換時に送信されない問題を修正
- `/skills` で Enter キーが `/<skill-name>` をプロンプトにプリフィルする代わりにダイアログを閉じる問題を修正
- `/agents` の詳細ビューでサブエージェントが利用できないビルトインツールを「Unrecognized」と誤ラベルする問題を修正
- プラグインキャッシュが不完全な場合に Windows でプラグインの MCP サーバーが起動しない問題を修正
- `/export` が会話で実際に使用したモデルではなく現在のデフォルトモデルを表示する問題を修正
- verbose 出力設定が再起動後に永続化されない問題を修正
- `/usage` のプログレスバーが「Resets …」ラベルと重なる問題を修正
- `${user_config.*}` が空のままのオプショナルフィールドを参照した際にプラグイン MCP サーバーが失敗する問題を修正
- 文末の数字を含むリストアイテムで数字が独自の行に折り返される問題を修正
- `/plan` および `/plan open` がプランモード進入時に既存のプランに基づいて動作しない問題を修正
- 自動コンパクション前に呼び出されたスキルが次のユーザーメッセージに対して再実行される問題を修正
- `/reload-plugins` と `/doctor` が無効化されたプラグインのロードエラーを報告する問題を修正
- `isolation: "worktree"` 付き Agent ツールが以前のセッションの古いワークツリーを再利用する問題を修正
- 無効化された MCP サーバーが `/status` で「failed」と表示される問題を修正
- `TaskList` がタスクを ID 順ではなく任意のファイルシステム順で返す問題を修正
- `gh` の出力に「rate limit」を含む PR タイトルがある際に不正な「GitHub API rate limit exceeded」ヒントが表示される問題を修正
- SDK/ブリッジの `read_file` が増大するファイルのサイズ上限を正しく適用しない問題を修正
- git ワークツリーで作業中に PR がセッションにリンクされない問題を修正
- `/doctor` が上位の優先スコープで上書きされた MCP サーバーエントリについて警告する問題を修正
- Windows: 誤った「Windows requires 'cmd /c' wrapper」MCP 設定警告を削除
- [VSCode] macOS でマイクパーミッションプロンプト表示中に音声ディクテーションの最初の録音が何も生成しない問題を修正

[参考リンク](https://code.claude.com/docs/en/changelog)
