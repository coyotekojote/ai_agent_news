## ツール実行時間のライブカウンター追加

折りたたまれたツールサマリー行にライブ経過時間カウンターが追加され、長時間実行されるツール呼び出しが停止しているように見えなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 権限ルールの起動時警告追加

`Write(path)`、`NotebookEdit(path)`、`Glob(path)` の権限ルールに対する起動時警告が追加された。代わりに `Edit(path)` または `Read(path)` の使用が推奨される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## worktreeサブエージェントのgitコマンド実行先修正

`isolation: 'worktree'` サブエージェントが、分離されたワークツリーではなくメインリポジトリのチェックアウトに対してgit変更コマンドを実行できてしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ultracodeキーワードの誤発動修正

`ultracode` キーワードオプトインが、Webhookペイロードや転送されたPRコメントなど人間以外の入力で発動してしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## クラッシュテレメトリへのテキスト漏洩修正

UIコンポーネントがスタイル付きテキスト要素の外側にコンテンツを返した際、レンダリングされたテキストフラグメントがクラッシュテレメトリに漏洩する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 外部エディタへのペーストマーカー漏洩修正

Claude Codeから開いた外部エディタにペーストマーカーが漏洩し、貼り付けたテキストの周囲に不正な文字（È/É）が表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude attachのセッション遷移時エラー修正

セッション遷移中に `claude attach` が「job not found」や「agent is still starting」エラーで失敗することがある問題が修正された。attachがデーモンの安定を待機するようになり、遅いattach中のターミナルリサイズも完了後に適用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ツール結果レンダラーのクラッシュ修正

ツールの結果レンダラーがUI要素の代わりにbigint数値やプレーンテキストを返した際にセッションがクラッシュする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フックタイムアウトの誤報告修正

フックコールバックのタイムアウトがモデルにユーザー拒否として誤って報告され、無人セッションが停止して待機してしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## cdコマンドのバックグラウンド移動時の動作修正

コマンドがバックグラウンドに移動された後も `cd` が有効になったとClaudeが想定してしまう問題が修正された。ツール結果で作業ディレクトリが変更されていないことが明示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインMCPサーバーの再同期時切断修正

セッション中にMCPサーバーが再同期された際、プラグイン提供のMCPサーバーが切断されてしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラン承認時のラベル誤表示修正

編集なしのプラン承認が「(edited by user)」とラベル付けされ、古いスナップショットでプランファイルが上書きされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /doctorのautoモード提案スキップ修正

Bedrock、Vertex、Foundryで `/doctor` が自動モードデフォルト提案をスキップしてしまう問題が修正された。これらの環境ではautoモードにオプトインが不要になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Grepコンテンツモードのページネーション修正

Grepコンテンツモードで結果の末尾を超えてページネーションした際に「No matches found」と誤表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 位置プレースホルダーのサイレント削除修正

スキルやコマンド内の未一致の `$1`/`$2` 位置プレースホルダーがサイレントに削除されていた問題が修正され、そのまま保持されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインキャッシュの一時ファイル残存修正

プラグインキャッシュの書き込み失敗時に一時ファイルが残る問題、およびWindowsとネットワークファイルシステムでロックされたファイルのリネームが失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドワーカーのクラッシュループ修正

クライアントがバックグラウンドサービスへの接続をリセットした際にバックグラウンドワーカーがクラッシュループする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agents --effort ultracodeの値伝達修正

`claude agents --effort ultracode` がディスパッチされたセッションに到達せず、値がサイレントに削除されていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビュー遷移時のタスクトラッカー消失修正

←キーでエージェントビューを開いた後セッションに戻る際にタスクトラッカーが消える問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントダッシュボードの画像保持修正

エージェントダッシュボードが、セッション削除後も放棄された返信ドラフトから貼り付けた画像を保持し続ける問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## git worktree lockの残存修正

強制終了されたバックグラウンドセッションが永続的な `git worktree lock` を残す問題が修正された。定期スイープが、所有プロセスが存在しないロックを解放するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## SDK MCPサーバーの接続遅延修正

`initialize` コントロールリクエスト経由で登録されたSDK MCPサーバーが、次のターンまで接続開始を待ってしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 代替スクリーン無効時のゴーストフレーム修正

`CLAUDE_CODE_DISABLE_ALTERNATE_SCREEN=1` でセッションからエージェントビューに戻る際に重なったゴーストフレームが残る問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## .claudeシンボリックリンクのサンドボックス反映修正

遅れて出現する `.claude/*` シンボリックリンクがサンドボックスの書き込み拒否リストに反映されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 間接的プロンプトインジェクション対策の強化

サブエージェントが読み取ったコンテンツを介した間接的なプロンプトインジェクションに対してAgentツールが強化された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bash/PowerShellツールのタイムアウトメッセージ改善

コマンドがタイムアウトして自動的にバックグラウンド化された際のBash/PowerShellツールメッセージが改善され、モデルがハングと明示的なバックグラウンド要求を区別できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## autoモードの権限分類器改善

autoモードの権限分類器が外部セッションでSonnet 5をデフォルトに使用するようになった。セッションの最初のリクエストで検証され、セッション中固定される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## datavizスキルのカラー検証改善

バンドルされたdatavizスキルのチャートカラー検証が、知覚的OKLab色差と再較正された色覚異常閾値で改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MEMORY.mdの読み取り制限超過時のエラー明示化

MEMORY.mdインデックスが読み取り制限を超えるメモリ書き込みが、サイレントな切り捨てではなく明示的なエラーを生成するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スクリーンリーダーモードの権限変更読み上げ

スクリーンリーダーモードで、Shift+Tabでモードを切り替える際に権限モードの変更が音声で読み上げられるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントフッターの入力待ち表示追加

エージェントフッターのヒントが、入力待ちのバックグラウンドエージェント数を表示するようになった。カウント変更時に短い色強調が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューのセッションマーク維持

エージェントビューで←キーから開いたセッションが、マウスホバーや矢印キーで選択が移動した後も視覚的にマークされたまま維持されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Fableアドバイザーの一時的利用不可表示

Fableアドバイザーの障害を引き起こすサーバー側の問題が修正されるまで、アドバイザーピッカーでFableが一時的に利用不可と表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)
