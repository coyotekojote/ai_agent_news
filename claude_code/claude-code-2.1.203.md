## ログイン有効期限の警告追加

ログインの有効期限が近づいた際に警告が表示されるようになり、バックグラウンドセッションが中断される前に再認証できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## 手動権限モードのバッジ表示追加

手動権限モードの際にフッターにグレーの一時停止バッジが表示されるようになり、アクティブなモードが常に確認できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## MCP roots/listへの追加作業ディレクトリの反映

セッションの追加作業ディレクトリがMCPの`roots/list`に追加され、セットが変更された際に`notifications/roots/list_changed`が送信されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## macOSでのバックグラウンドエージェントセッション切り替え遅延の修正

macOSでバックグラウンドエージェントセッションの開始や切り替えが偽の低メモリ検出により15〜20秒停止する問題が修正された（2.1.196でのリグレッション）。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## バックグラウンドセッションの無応答修正

デーモンのセッショントークンが失効した際にバックグラウンドセッションがアタッチ、リプライ、停止に対して永久に無応答になる問題が修正された。セッションは自動的に回復するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## `claude agents`復帰時のサブエージェント停止修正

`claude agents`に戻る際に実行中のサブエージェントが暗黙的に停止され、プロンプトが最初からやり直される問題が修正された。作業が引き継がれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## インタラクティブセッションのメモリ・CPU使用量リグレッション修正

インタラクティブセッションにおけるメモリおよびターンごとのCPU使用量のリグレッションが修正された。コンテキスト使用量インジケーターが毎ターン後にトランスクリプト全体を再分析しなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## バックグラウンドエージェントのPATH継承修正

バックグラウンドエージェントがディスパッチシェルではなくデーモンから古い`PATH`を継承し、Windowsでツールが見つからなくなる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## `ANTHROPIC_BASE_URL`の欠落修正

バックグラウンドおよびエージェントビューセッションがシェルからエクスポートされた`ANTHROPIC_BASE_URL`を欠落させ、APIキーがデフォルトエンドポイントに送信されて401エラーで失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## 多数のworktreeでのBashエラー修正

多数のgit worktreeを持つリポジトリでBashが「argument list too long」で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## worktree分離サブエージェントのシェルコマンド実行ディレクトリ修正

worktreeで分離されたサブエージェントが、自身のworktreeではなく親チェックアウトでシェルコマンドを実行してしまう問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## マルチリポジトリワークスペースでのworktree作成修正

マルチリポジトリワークスペースでネストされたリポジトリを拒否するworktree作成の問題が修正され、バックグラウンドセッションが分離・編集できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## バックグラウンドエージェントの作業ディレクトリ削除時のクラッシュループ修正

バックグラウンドエージェントの作業ディレクトリが削除、ファイルに置き換え、または無効なパスになった際にクラッシュループに陥る問題が修正された。明確なエラーで一度だけ失敗するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## デーモン自動アップグレード失敗時のセッション停止修正

バックグラウンドデーモンの自動アップグレード失敗が全ての実行中バックグラウンドセッションを暗黙的に停止させる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## TaskStop・TaskOutputの他エージェントからの検索修正

別のエージェントが起動したバックグラウンドエージェントを`TaskStop`や`TaskOutput`が見つけられない問題が修正された。エラーは実行中のエージェントをIDと説明でリスト表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## `claude agents`コンポーザーのメッセージ破棄修正

`claude agents`のコンポーザーで、スラッシュコマンドが利用できない場合に入力済みメッセージが破棄される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## 停止済みセッションのエージェントリストクラッシュ修正

会話が既に別のセッションで開かれている停止済みセッションを開く際にエージェントリストがクラッシュする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## バックグラウンドセッションの「Needs input」表示修正

バックグラウンドセッションが質問への回答後もエージェントリストで「Needs input」と表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## バックグラウンドエージェント起動失敗のエラー表示修正

バックグラウンドエージェントの起動失敗が実際のエラーではなく「exit_with_message」のみ表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## バックグラウンドセッションのeffortLevel設定反映修正

デーモン経由でフォークされた際にバックグラウンドセッションがsettings.jsonの`effortLevel`の変更を無視する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## アタッチ済みバックグラウンドセッションのマウス無効化修正

アタッチされたバックグラウンドセッションが`CLAUDE_CODE_DISABLE_MOUSE`および`CLAUDE_CODE_DISABLE_MOUSE_CLICKS`のオプトアウトを無視する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## `/exit`のバックグラウンドエージェント警告修正

全ての名前付きエージェントが完了した後も`/exit`がバックグラウンドエージェントの実行について誤って警告する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## 非gitディレクトリからのバックグラウンドセッション起動修正

非gitディレクトリから起動されたバックグラウンドセッションが`WorktreeCreate`フックが設定されている場合にファイルを編集できない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## `claude agents`の`@`ディレクトリピッカー修正

`claude agents`の`@`ディレクトリピッカーが登録されたgit worktreeを表示しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## Windowsでのバックグラウンドタスク出力修正

Windowsでバックグラウンドタスクの出力が`/clear`後に空ファイルに永久に置き換えられる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## 長いトランスクリプト履歴のスクロール時のコンテンツジャンプ修正

長いトランスクリプト履歴を上方にスクロールする際のコンテンツジャンプが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## bashモードでのターミナルフリッカー修正

bashモードでシェル履歴の候補が表示されている際の入力時にターミナルがちらつき、ジャンプする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## バックグラウンドセッション再アタッチ時のエスケープコード修正

バックグラウンドセッションに再アタッチする際にリテラルの`^[[I]`/`^[[O]`エスケープコードが出力される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## LSP専用プラグインの不使用フラグ修正

言語サーバーが診断やナビゲーションリクエストに応答しているLSP専用プラグインが誤って不使用としてフラグ付けされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## ストリーミング中のレスポンシブ性向上

長いレスポンスのストリーミング中のレスポンシブ性が向上した。ライブプレビューの更新が画面全体を再レンダリングしなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## サブエージェントの再委任抑制

エージェントがタスク全体を別のサブエージェントに再委任する可能性が低くなった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## バイナリサイズとメモリ使用量の削減

大きなバンドル依存関係の遅延読み込みにより、バイナリサイズが約7MB、起動時メモリが約7MB削減された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## 左矢印キーの動作変更

左矢印キーがバックグラウンドタスク、diff、ワークフロー詳細ビューを閉じなくなった。代わりにEscを使用する。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## 空の`claude agents`ビューの改善

空の`claude agents`ビューが常に整理されたセクション（Needs input / Working / Completed）と説明を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## 起動時警告の移動

起動時の「claude command missing or broken」警告が削除され、`/doctor`および`/status`に表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)

## VSCode Remote Control設定トグルの追加

VSCodeに「Enable Remote Control for all sessions」の設定トグルが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.203)
