## フォールバックモデル設定

`fallbackModel`設定が追加され、プライマリモデルが過負荷または利用不可の場合に試行する最大3つのフォールバックモデルを順序付きで構成できるようになった。`--fallback-model`がインタラクティブセッションにも適用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## deny/allowルールのglobパターンサポート

denyルールのツール名位置でglobパターン（`"*"`で全ツール拒否）がサポートされた。allowルールは非MCPのglobを拒否し、denyルール内の不明なツール名は起動時に警告が表示される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## クロスセッションメッセージングの強化

`SendMessage`経由で他のClaudeセッションから中継されたメッセージがユーザー権限を持たなくなった。受信側は中継された権限リクエストを拒否し、autoモードではブロックされる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## thinking無効化の制御

`MAX_THINKING_TOKENS=0`、`--thinking disabled`、およびモデルごとのthinkingトグルにより、デフォルトでthinkingを行うモデルでClaude API経由でthinkingを無効化できるようになった（サードパーティプロバイダーは変更なし）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フォールバックモデルでの自動リトライ

APIが予期しない非リトライ可能エラーを返した場合、フォールバックモデルで1回自動リトライされるようになった。認証、レート制限、リクエストサイズ、トランスポートエラーは即座に表示される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude updateの改善

`claude update`がダウンロード前にターゲットバージョンを表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsのURL検索

`claude agents`でリストにURLを入力すると、最初のプロンプトにそのURLが含まれるセッションにフィルタリングされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

セッション内で処理不可能な画像が送信された際の「image could not be processed」エラーの繰り返しと余分なトークン消費が修正された。

ワーカー登録時のバックエンド障害でリモートセッションが永久にスタックする問題が修正された。

JetBrains IDEターミナル（IntelliJ、PyCharm、WebStorm等）の2026.1以降でのちらつきが、同期出力の有効化により修正された。

Kittyキーボードプロトコルを使用するターミナル（WezTerm、Ghostty、kitty）でShift+非ASCII文字（例：Shift+ä→Ä）が無視される問題が修正された。

WindowsでPowerShellコマンド検証が、killされたプロセスの子プロセスが出力パイプを保持している場合にタイムアウトを大幅に超えてハングする問題が修正された。

macOSでデーモンが接続中に死亡した後、`claude --bg-pty-host`プロセスが孤立してCPU 100%で回転する問題が修正された。

`/voice`トグル後にvoiceモードが`/login`を必要とする古い認証チェックの問題が修正された。

無効なエントリを持つmanaged settingsが残りの有効なポリシーの適用を暗黙的に無効化する問題が修正された。

managed-settingsの`allowedMcpServers`/`deniedMcpServers`述語が`${VAR}`参照使用時にマッチしない問題が修正された。

git worktreeでクラッシュループしていたバックグラウンドエージェントセッションが「No conversation found」で`claude agents`から再開できない問題が修正された。

ストリーミング中のCtrl+Oトランスクリプトビューでthinkingテキストが重複表示される問題が修正された。

リモートセッション内で`/doctor`が矛盾する「Not inside a remote session」チェック失敗を表示する問題が修正された。

`claude agents`のディスパッチ・リプライ入力でマルチラインプロンプト入力時にカーソルが最初の行末に固定される問題が修正された。

Unicode未対応ターミナルでタスクリストのバックグラウンドエージェント行間に空白行が表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)
