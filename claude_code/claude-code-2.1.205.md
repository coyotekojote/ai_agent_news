## セッショントランスクリプトファイルの改ざん防止

セッショントランスクリプトファイルの改ざんをブロックする自動モードルールが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## `--json-schema`の無効スキーマ処理修正

`--json-schema`でスキーマが無効な場合に非構造化出力が暗黙的に生成される問題と、`format`キーワードを使用するスキーマが拒否される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## `--max-turns`制限時のメッセージ消失修正

Claudeの作業中に送信されたメッセージが、ターンが`--max-turns`制限で終了した際に暗黙的に失われる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## Windows worktree削除時のファイル誤削除修正

NTFSジャンクションまたはディレクトリシンボリックリンクがworktree内に存在する場合、Windows worktreeの削除がworktree外のファイルを削除してしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## バックグラウンドエージェントの再開後ステータス表示修正

`SendMessage`で再開した後もバックグラウンドエージェントがエージェントリストで「failed」や「completed」と表示され続ける問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## バックグラウンドジョブのステータス表示修正

エージェントのターンに読み取り可能なテキストがない場合、バックグラウンドジョブがエージェントリストで「needs input」から「working」に戻ってしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## `claude attach`のアップグレード再起動中エラー修正

バックグラウンドエージェントがアップグレード再起動中の場合に`claude attach`がエラーになる問題が修正され、復帰を待機するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## セッションからPRへのリンク修正

Bash呼び出しの出力が30Kインライン制限を超えた場合にセッションからPRへのリンクが欠落する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## `claude mcp add-from-claude-desktop`のスタック修正

サーバー名にサポートされていない文字が含まれている場合に`claude mcp add-from-claude-desktop`がスタックする問題が修正された。無効な名前が報告され、残りのサーバーは引き続きインポートされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## プラグインLSPサーバーの初期化失敗修正

あるプラグインのLSPサーバーの初期化失敗が、同じファイル拡張子を処理する別のプラグインの有効なLSPサーバーの動作を妨げる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## Windowsでのディレクトリ削除時クラッシュ修正

Claudeの起動元ディレクトリがコマンド実行中に削除、ロック、またはアンマウントされた場合のWindowsクラッシュが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## ファイルウォッチャー終了時のクラッシュ修正

ディレクトリスキャンがまだ進行中にファイルウォッチャーが閉じられた際のクラッシュが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## プロジェクト検証スキルの不要な再書き込み修正

ドキュメント化されたコマンドが変更されていない場合でも、毎セッションでプロジェクト検証スキルが書き換えられる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## エージェントビューのレンダリング修正

ジョブリストが画面をわずかにオーバーフローした際に、エージェントビューが1行高く描画されヘッダーがクリッピングされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## WebおよびモバイルRemote Controlのステータス表示修正

WebおよびモバイルのRemote Controlパネルでバックグラウンドタスクが古い「Running」ステータスを表示する問題が修正され、メンバーシップ変更のたびに完全なタスク状態が転送されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## `rm -rf`実行前の確認改善

自動モードでコンテキストから解決できない変数に対する`rm -rf`実行前に確認を求めるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## 自動アップデートのメモリ使用量削減

自動アップデートのバイナリダウンロードがメモリにバッファリングする代わりにディスクにストリーミングされるようになり、アップデーターのピークメモリ使用量が約400MB削減された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## バックグラウンドタスク通知のセキュリティ強化

バックグラウンドタスクの通知が人間の入力がなかったことを明示的に示すようになり、トランスクリプト内の捏造された承認に基づく行動が防止された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## エージェントビューのPRリンク改善

セッションが既存のPRを編集、マージ、コメント、またはプッシュした場合、`claude agents`にPRがリンクされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## エージェントビューの表示改善

行に生のツールコールテキストではなく色付きの状態ワードと分類器が生成した見出しが表示されるようになった。ピークではブロックされたセッションの正確な質問を含む完全なステータスが開かれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## `/doctor`コマンドの強化

`/doctor`がセットアップの問題を診断・修正できる完全なセットアップチェックアップになった。`/checkup`がそのエイリアスとして追加された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## MCPサーバー名の予約

Claude Desktopペインの名前変更に先立ち、「Claude Browser」MCPサーバー名が「Claude Preview」と並んで予約された。ユーザー設定のMCPサーバーはいずれの名前でも登録できなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)

## Cowork VMモードのログインエラー修正

CLI 2.1.203以降でCowork VMモードのローカルエージェントセッションが「Not logged in · Please run /login」で起動に失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.205)
