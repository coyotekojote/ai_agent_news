## `agentStop`フックの無限ループ防止

`agentStop`フックが常にブロックする場合に無限ループしなくなった。CLIは8回連続ブロック後にターンを終了し、`agentStop`フックは`stop_hook_active`フラグを受け取ることで強制継続を検出して自己制限できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## OSサンドボックスでのgit/gh認証のオプトイン

OSサンドボックス内でgitおよびgh認証をオプトインで使用できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## サンドボックスmacOSキーチェーンアクセスのデフォルトオフ

サンドボックスのmacOSキーチェーンアクセスがデフォルトでオフになり、分離性が向上した。必要に応じて`/sandbox`で再有効化できる。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## ライフサイクル・サブエージェントフックの実行ディレクトリ修正

ライフサイクルフックとサブエージェントフックのコマンドが`/cd`後の現在のセッションディレクトリで実行されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## MCPサーバー削除時のプロセス停止

`/mcp delete`でMCPサーバーを削除すると、実行中のバックグラウンドプロセスも停止するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## `/sandbox`トグル時のMCPサーバー再起動の最適化

`/sandbox`のトグル時にローカルMCPサーバーのみ再起動し、リモートサーバーは接続を維持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## `/cd`後のコマンド承認のリセット

`/cd`でリポジトリを切り替えた後、コマンド承認が別のリポジトリに引き継がれなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## WindowsでのGitHubタブのブラウザ起動修正

GitHubタブの「Open in web」アクションがWindows上で確実にブラウザを起動するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## モデル変更時の貼り付けプロンプト内容の保持

`Ctrl+X /model`でモデルを変更する際に、貼り付けたプロンプト内容が保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## ファイル作成時の行数カウント修正

ファイル作成時に表示される追加行数が修正され、末尾に改行があるファイルで1行多く報告されなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## ワークツリー作成の信頼性向上

`/worktree`と`/move`が、類似名のブランチや残留ワークツリーディレクトリが存在する場合でも自動生成ブランチ名でワークツリーを作成できるようになった。`/worktree`がキックオフタスクをメインリポジトリで実行してしまう間欠的な問題が修正された。また、ソースが信頼済みの場合にフォルダ信頼が新しいワークツリーに伝播され、`/move`はgit stashを正確に処理するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## セッション表示の改善

ワークスペースがキャッシュスナップショットのみで利用可能な場合、メッセージのないリネーム済みセッションに終了再開ヒントが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## MCPサーバー接続メッセージの表示

遅いMCPサーバーが最終的に接続した際に接続メッセージが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## `/plugins`コマンドの拡張

`/plugins`に`update`/`uninstall`動詞が追加された。`enable`/`disable`/`remove`が`--plugin`/`--mcp`/`--skill`フラグまたは位置引数でプラグイン、MCPサーバー、スキルをターゲットにできるようになった。`/plugins install --skill`でスキルのインストールがサポートされた。`/plugins help`コマンドも追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## セッションエクスポートのフォーマット改善

セッションエクスポートでインラインコードとトップレベルのフェンス付きコードブロック内の山括弧がそのまま保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## MCPサーバーステータス表示の修正

`constructor`や`__proto__`のような名前のMCPサーバーのステータスが正しく表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## セッションハイライトの改善

セッションを閉じた際に、分割ビューとスタンドアロンのセッションタブの両方で最も近いライブ行にハイライトが維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## インラインHexカラーコードのスウォッチ表示

インラインコードで記述されたHexカラーコード（例：`#FF0000`）がカラースウォッチとして表示されるようになった。`renderHexColors`設定（デフォルトオン）でトグルできる。Markdownリスト内でのスウォッチのパディングも修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## インタラクティブシェルショートカット

プロンプトで`$`を入力すると現在のセッションディレクトリでインタラクティブシェルが開くようになった。`/settings shellShortcut on`で有効化でき、デフォルトはオフ。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## ネストされたMarkdownリストの正しいレンダリング

バッファ出力（`-p --stream off`および詳細画面）でネストされたMarkdownリストが正しくレンダリングされるようになった。サブ箇条書きが親項目の行に結合されたりフラット化されたりせず、親の下にインデントされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## スキル一覧のターミナル制御文字除去

`copilot skill list`がスキル名と説明からターミナル制御文字を除去するようになり、細工されたスキルがANSIエスケープシーケンスを一覧出力に注入できなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## CLIからのスキルインストール

`copilot plugins install --skill <file, URL, or directory>`でスキルをインストールできるようになった。`--scope project`を追加するとリポジトリにインストールされる。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## `/settings`のデフォルト値表示とブール値サイクル

`/settings`でデフォルト値が表示されるようになり、ブール値がデフォルトに戻るサイクルが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## リモートコントロールのSSO要求

管理設定で要求されている場合、リモートコントロールにSSOが必須となった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## `/settings show`でのシークレット値マスキング

`/settings show`出力でシークレット値がマスクされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## `/model --session`の追加

`/model --session`（`-s`）が追加され、現在のセッションのみのモデル、推論努力、コンテキストウィンドウを変更でき、グローバル設定は変更されないようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## `/terminal-setup`のエディタ検出改善

`/terminal-setup`がVS Code、Cursor、Windsurfを親プロセスから検出するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## セッションサイドバーのキーボード・マウスナビゲーション

セッションサイドバーがキーボードとマウスで操作可能になった。矢印キーで選択を移動し、Enterまたはクリックでセッションを切り替える。`n`で新規セッション、`x`を2回押してセッションを閉じることができる。`/settings`で無効化や記憶済みセッションの復元停止が可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## マルチターンサブエージェントの常時有効化

マルチターンサブエージェントが常に有効になり、実行中のエージェントにフォローアップメッセージを送信できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## Claude Haiku 4.5+のツール検索サポート

Claude Haiku 4.5以降でツール検索が有効になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## 絵文字ショートコードのフォーマット修正

絵文字ショートコード（例：🎉）がプリント出力やPR/Issue/Gist出力で末尾に不要なスペースを付けなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)

## スケジュールプロンプトのステアリングメッセージ配信

エージェントがビジー状態の場合、スケジュールされたプロンプトがステアリングメッセージとして配信されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72)
