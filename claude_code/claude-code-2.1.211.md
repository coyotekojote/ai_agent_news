## サブエージェントテキストのストリーム出力転送フラグ追加

`--forward-subagent-text` フラグおよび `CLAUDE_CODE_FORWARD_SUBAGENT_TEXT` 環境変数が追加され、サブエージェントのテキストとthinkingをstream-json出力に含められるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 権限プレビューの双方向オーバーライド文字無害化

チャットチャネルに中継される権限プレビューが、双方向オーバーライド、ゼロ幅、類似引用文字を無害化するようになり、ツール入力が承認メッセージを視覚的に改変できなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## autoモードのPreToolUseフックask決定の上書き修正

autoモードがサンドボックス外Bashに対するPreToolUseフックの `ask` 決定を上書きしてしまう問題が修正された。フックの `ask` がプロンプト表示を最低限保証するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スリープ復帰時の並列セッション同時ログアウト修正

多数のセッションが1つの認証情報ストアを共有している場合、スリープ復帰後にすべてのClaude Codeセッションが同時にログアウトしてしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインMCPサーバーのアイドルWebセッション復帰時再接続修正

アイドル状態のWebセッションが復帰した際にプラグインMCPサーバーが再接続されず、次のメッセージまでMCP呼び出しが失敗し続ける問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vertex/Bedrockでの起動時フォールバック通知修正

Vertex/Bedrock上のClaude Codeが起動時にデフォルトのOpusモデルを試行し、モデルが明示的に設定されている場合でも偽のフォールバック通知を表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントのモデルオーバーライド復帰修正

明示的なモデルオーバーライドで起動されたサブエージェントが、再開時やフォローアップメッセージ送信時に親のモデルに戻ってしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネストされた.claude/rulesファイルの読み込み制限修正

設定ソースがプロジェクト設定を除外している場合でも、ネストされた `.claude/rules/*.md` ファイルが読み込まれてしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ファイルアップロードバリデーションの修正

DOSデバイスサフィックス（`.prn`）や末尾ドットで終わるファイル名が受け入れられるようになり、複数のハードリンクを持つファイルは拒否されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Chromeからのファイルアップロードの修正

リモートおよびCLIセッションからのChrome経由のファイルアップロードが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 入力が「?」になる編集のサイレント消失修正

入力を「?」のままにする編集がサイレントに消失し、ショートカットパネルがトグルされてしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Chrome拡張機能有効時のChromeなし起動ハング修正

Claude in Chrome拡張機能が有効でChrome未起動の場合に起動がハングする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 非同期コンテンツの300ms表示遅延修正

設定タブ、統計、diffビュー、その他のローディング状態などの非同期コンテンツが表示されるまでの300ms遅延が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 停止直後のバックグラウンドセッション再開時の空白会話修正

エージェントビューから停止直後のバックグラウンドセッションを再開すると、同じセッションIDで空白の会話が開始される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /loopの/resume非表示修正

`/loop` を一度使用した後にセッションが `/resume` から非表示になる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スクリーンリーダーのターミナルベル消失修正

スクリーンリーダーユーザーが `/terminal-setup` またはオンボーディングのターミナルセットアップ後に聴覚的ターミナルベルを失う問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## LLMゲートウェイ認証のバックグラウンドジョブ修正

LLMゲートウェイ認証（`ANTHROPIC_AUTH_TOKEN` + `ANTHROPIC_BASE_URL`）でバックグラウンドジョブがデーモン再起動後に「Not logged in」と表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsのworktree認識不能時の削除不可修正

gitがworktreeを認識できなくなった場合に `claude agents` のジョブが永続的に削除不可能になる問題が修正された。サイレントに再表示される代わりに、削除が拒否された理由が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /clearのセッションコストカウンターリセット修正

`/clear` がセッションのコストカウンターをリセットしない問題が修正された。`/clear` 後にステータスラインのコストが$0から開始されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Claude in ChromeのWindowsセットアップページ修正

WindowsでClaude in Chromeのセットアップページがブラウザで開けない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windowsのヘッドレス印刷モードセッション修正

stdinが読み取り不可能な場合にWindowsのヘッドレス印刷モードセッションがクラッシュまたはサイレント終了する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションタイトルの拒否テキスト表示修正

プロンプトにリンクが含まれる場合にエージェントビューのバックグラウンドセッションタイトルが命名モデルの拒否テキストを表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントの自動再起動・古いプロンプト再実行修正

ユーザーによって終了されたバックグラウンドエージェントが自動再起動する問題、および復活したエージェントが古いセッションの古いプロンプトを再実行する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スケジュールなしルーティンの次回実行時刻修正

スケジュールが設定されていないルーティンが西暦1年の次回実行時刻を報告する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windowsでの同期スキル/プラグインディレクトリ命名の堅牢化

Windowsでの同期スキル/プラグインディレクトリの命名が堅牢化され、CCR Web fetch/searchプロキシが `/clear` 後も動作し続けるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ターミナルレイアウトとレンダリングパフォーマンスの改善

ターミナルのレイアウトとレンダリングパフォーマンスが改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェント結果報告の改善

バックグラウンドエージェントの結果報告が改善された。Claudeが実行中のエージェントのステータスを報告し、結果を捏造する代わりに実際の完了を待つようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## メモリインデックス超過警告の改善

メモリインデックスの超過警告が、フロントマターとHTMLコメントを除外し、読み込まれたコンテンツのみを測定するように改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 整数環境変数の科学的記数法サポート

整数環境変数（タイムアウト、トークンバジェット、リトライ回数）が `1e6` や `64_000` のような科学的記数法やdigit-separator表記を受け入れるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ドキュメントリンクの更新

ドキュメントリンクが最新のドキュメントサイトに更新された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 「always allow」権限ルールのリポジトリルート保存

「always allow」権限ルールがリポジトリルートに保存されるようになり、git worktreeで付与された承認がセッションやworktree間で永続化されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /usage-creditsの確認プロンプト追加

`/usage-credits` が組織管理者にリクエストを送信する前に確認を求めるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vimモードのs/Sキー動作修正

Vimモードの `s`（文字置換）と `S`（行置換）がNORMALモードで動作するようになり、vimの動作に一致するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## VSCode Remote Controlバナーの更新

VSCodeのRemote Controlバナーが機能の説明を含むように更新された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Claude in Chromeのファイルアップロードパス検証強化

Claude in Chromeのファイルアップロードパス検証が強化された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Claude in Chromeのスクリーンショットsave_to_disk修正

スクリーンショットアクションの `save_to_disk` がディスクに画像を書き込みパスを返すようになった。以前は何も行わなかった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrock/Vertex/Mantle/Foundryのプロンプトキャッシュ回帰修正

Bedrock、Vertex、Mantle、Foundryにおいて、末尾のシステムコンテキストブロックが毎回のリクエストで新規入力トークンとして課金されるプロンプトキャッシュの回帰が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)
