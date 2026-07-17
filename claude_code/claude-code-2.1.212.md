## `/fork`がバックグラウンドセッションへの会話コピーに変更

`/fork`が会話を新しいバックグラウンドセッション（`claude agents`に独自の行として表示）にコピーするように変更された。以前のインセッションサブエージェント起動機能は`/subtask`に移行された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude auto-mode reset`コマンドの追加

デフォルトのauto-mode設定を復元する`claude auto-mode reset`コマンドが追加された。確認プロンプト付きで、`--yes`でスキップ可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WebSearch呼び出しのセッション単位制限追加

暴走する検索ループを防止するため、WebSearchツール呼び出しにセッション単位の制限（デフォルト200回）が追加された。`CLAUDE_CODE_MAX_WEB_SEARCHES_PER_SESSION`で調整可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェント生成のセッション単位キャップ追加

暴走する委任ループを防止するため、サブエージェント生成にセッション単位のキャップ（デフォルト200、`CLAUDE_CODE_MAX_SUBAGENTS_PER_SESSION`でオーバーライド可能）が追加された。`/clear`でバジェットがリセットされる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPツール呼び出しの自動バックグラウンド移行

2分以上実行されるMCPツール呼び出しが自動的にバックグラウンドに移行され、セッションが使用可能な状態を維持するようになった。`CLAUDE_CODE_MCP_AUTO_BACKGROUND_MS`で閾値の設定または無効化が可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/resume`のエージェントビューでのセッションピッカー追加

エージェントビューで`/resume`を入力すると、リストから削除されたセッションを含む過去のセッションのピッカーが表示され、選択したセッションをバックグラウンドセッションとして再開できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プランモードでのファイル変更Bashコマンド自動実行の修正

プランモードがファイルを変更するBashコマンド（`touch`、`rm`など）を権限プロンプトやSDK `canUseTool`コールバックなしで自動実行する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `.claude/worktrees`シンボリックリンクによるworktree作成の修正

リポジトリにコミットされた`.claude/worktrees`のシンボリックリンクに従ってworktreeが作成され、リポジトリ外にファイルが作成される可能性がある問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `continue:false`フックの停止がドロップされる問題の修正

ツールが失敗または完了した際に`continue:false`フックの停止がドロップされ、フックインフラストラクチャのエラーがユーザー拒否として誤報告される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bashツール実行中のSIGTERMでのプロセスツリー孤立修正

print/SDKモードで実行中のBashツールに対するSIGTERMがコマンドのプロセスツリーを孤立させる問題が修正された。CLIがターンを中断し、ツリーをキルし、143で終了するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windowsでの`/background`と`claude --bg`の失敗修正

グループポリシーがPowerShell 5.1をブロックしている場合にWindowsで`/background`と`claude --bg`が「EUNKNOWN: unknown error, uv_spawn」エラーで失敗する問題が修正された。デーモンがPowerShell 7を優先するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## シェルモードでのファイルパスを含むコマンド実行の修正

パスオートコンプリートポップアップが開いている状態でシェルモード（`!`）がファイルパスを含むコマンドを実行しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## auto-mode拒否通知の文字化け修正

長い拒否理由が絵文字の途中で切り捨てられた場合にauto-mode拒否通知が文字化けする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューでのCtrl+J改行挿入の修正

拡張キーレポーティングを使用するターミナルでエージェントビューのディスパッチ入力にCtrl+Jで改行が挿入されない問題が修正され、`?`ヘルプオーバーレイに改行ショートカットが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/ultrareview`のPR参照拒否の修正

`/ultrareview`が`#123`、`PR 123`、貼り付けられたPR URLなどのPR参照を拒否する問題が修正された。エラーヒントが実際に入力したコマンド名を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/ultrareview`のリモートブランチ未取得の修正

`/ultrareview <branch>`がリモートに存在するブランチをoriginから取得しない問題が修正された。タイプミス時に最も近いブランチ名を提案するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/ultrareview`の課金確認スキップの修正

`/clear`後の新しい会話で`/ultrareview`が課金確認をスキップする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/ultrareview`のClaude Desktopでのエラー修正

Claude Desktopでの`/ultrareview`の「not a git repository」エラーが、ターミナルコマンドの代わりにプロジェクトのリポジトリフォルダを提案するように修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ホスト管理セッションの起動時失敗の修正

リポジトリ設定でmTLS証明書、追加CAバンドル、またはOAuthスコープが設定されている場合にホスト管理セッションが起動時に失敗する問題が修正された。これらのトランスポート設定は警告とともに無視されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッション再開時の「File has not been read yet」エラー修正

offset/limitでファイルを読み取った後にセッションを再開すると偽の「File has not been read yet」エラーが表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `ExitWorktree`のセッション再開後のエラー修正

print/SDKモードで`--continue`/`--resume`でセッションを再開した後に`ExitWorktree`が「no active EnterWorktree session」エラーで失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Controlクライアントのワークフローエージェントグリッド空表示修正

実行中のセッションに途中から参加したRemote Controlクライアントでワークフローエージェントグリッドが空のままになる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ストリーミングモードの制御リクエスト早期完了マーク修正

ストリーミングモードの制御リクエストがハンドラーの完了前に完了マークされ、セッション再起動時にリクエストが失われる可能性がある問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/fork`で作成されたバックグラウンドセッションの保護喪失修正

`/fork`で作成されたバックグラウンドセッションが状態書き込み失敗後にライブ親保護を失う問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 停止したバックグラウンドセッションの再開失敗修正

エージェントビューから停止したバックグラウンドセッションを再開する際にサイレントに失敗する問題が修正された。セッションが再開されるか、できない理由が表示され強制再起動が可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントチームの重複アイドル通知修正

停止中のチームメイトがチーム初期化がセッション内で再実行された際にリーダーに重複アイドル通知を送信する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラン承認ダイアログのフッター分割修正

ファイルパスが長い場合にプラン承認ダイアログのフッターの「ctrl+g to edit in `<editor>`」が分割される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フルスクリーンモードでのウェルカムバナーのパネル幅修正

フルスクリーンモードで幅と高さを同時にリサイズした後にウェルカムバナーが古いパネル幅を維持する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 狭いレイアウトでのdiffプレビューの行番号消失修正

狭いレイアウトでdiffプレビューの行番号と+/-マーカーが失われる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## @メンション・プラグインアンインストール・タイムアウト関連の修正

部分的なファイル読み取り後に@メンションが何も添付しない問題、プラグインアンインストールが間違ったマーケットプレースを対象にする問題、終了コード143での偽の「Command timed out」の問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OpenTelemetry HTTPエクスポートの拒否修正

Azure Monitorおよびチャンク転送エンコーディングを受け入れないエンドポイントでOpenTelemetry HTTPエクスポートが411/400で拒否される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OTLPイベントログレコードのtrace_id/span_id欠落修正

SDK/ヘッドレスモードで`TRACEPARENT`が設定されている場合にOTLPイベントログレコードの`trace_id`/`span_id`が欠落する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 多数の画像を含む会話の「Request too large」エラー修正

多数の画像を含む会話が誤って「Request too large」エラーで失敗する問題が修正され、実際の原因を説明するようエラーメッセージが改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Web検索・Web取得のAPIエラーテキスト返却修正

APIが過負荷の場合にWeb検索とWeb取得が「API Error」テキストを検索結果やページコンテンツとして返す問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Web検索・Web取得の信頼性向上

529エラーおよびレート制限されたリクエストに対してバウンド付きバックオフでリトライすることで、Web検索とWeb取得の信頼性が向上した。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プロンプトキャッシュの改善

会話途中のシステムブロックがLLMゲートウェイおよびカスタムベースURL（Bedrock、Vertex、1P）の背後でも動作するようプロンプトキャッシュが改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントアタッチの改善

コールドアタッチ時に、空白の待機状態の代わりにセッション起動中でもフォーマット済みのトランスクリプトが即座に表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェント間メッセージングのトークン使用量削減

`SendMessage`本文がリプレイされた履歴やツール結果に重複しなくなり、トークン使用量が削減された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/fork`のセッション命名改善

セッションにタイトルがない場合、`/fork`がプロンプトに基づいてコピーに名前を付けるようになり、エージェントビューで認識しやすくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/btw`のサイドクエスチョンパネル再表示

引数なしの`/btw`が最新のやり取りのサイドクエスチョンパネルを再表示し、以前の回答をブラウズできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェント完了時の左矢印フッターヒント更新

入力待ちがない状態でバックグラウンドエージェントが完了した際に、左矢印フッターヒントが一瞬`N done`とパルスするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Taskツールの`mode`パラメータ非推奨化

Taskツールの`mode`パラメータが非推奨化された（無視される）。サブエージェントはデフォルトで親セッションの権限モードを継承する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Enterprise `forceLoginMethod`の適用範囲拡大

Enterprise `forceLoginMethod`がターミナルだけでなく、VS Code拡張機能、SDK、`setup-token`、`install-github-app`ログインにも適用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッショントランスクリプトへのreasoning effortレベル記録

セッショントランスクリプトが各アシスタントメッセージにreasoning effortレベルを記録するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ヘッドレス/SDKセッションの`set_model`制御リクエストのターン中適用

ヘッドレス/SDKセッションが`set_model`制御リクエストをターン中に適用するようになり、次のモデルラウンドトリップで次のターンを待たずに新しいモデルが使用される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューの「Needs input」ステータス表示

エージェントビュー/`claude agents --json`で、サンドボックス、MCP入力、または管理設定プロンプトを待機中のセッションが「Working」ではなく「Needs input」と表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 認証ステータスパネルタイトルの更新

認証ステータスパネルのタイトルが「Cloud authentication」から「Authentication」に更新された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## tmux同期出力に関する以前のリリースノートの訂正

以前のリリースノート（2.1.200）が訂正された。tmuxは3.6シリーズまで同期出力を欠いており、対応するより新しいtmuxは自動的に検出される。

[参考リンク](https://code.claude.com/docs/en/changelog)
