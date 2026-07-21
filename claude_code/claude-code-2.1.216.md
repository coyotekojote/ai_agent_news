## `sandbox.filesystem.disabled`設定の追加

ファイルシステム分離をスキップしつつネットワーク出口制御を維持するための`sandbox.filesystem.disabled`設定が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 長時間セッションでのパフォーマンス低下の修正

メッセージ正規化コストがターン数に対して二次関数的に増大し、数秒のストールや遅いレジュームを引き起こしていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 自動モードでのOAuthトークン期限切れ時のコマンド拒否修正

OAuthトークンがセッション中に期限切れまたはローテーションされた後、「HTTP 401」分類エラーでコマンドが拒否されていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## AskUserQuestionの応答処理の修正

ユーザーが待機や説明を求めた回答に対しても、Claudeに継続するよう指示していた問題が修正された。自由テキスト回答に中立的な表現が使用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Web版Claude Codeのアイドル後の質問繰り返し修正

セッションが数分間アイドル状態になった後、同じ質問を再度表示して回答を破棄していた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## @メンション関連の複数修正

ファイル変更フック後に@メンションが何も添付しなくなる問題、vimのドットリピートや`c`オペレータ・貼り付け関連の問題、ステータスラインがレジューム時に二重実行される問題、レジュームピッカーが失敗時にハングする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントセッションのレジューム修正

レジュームされたバックグラウンドエージェントセッションがデフォルトエージェントに戻ってしまう問題が修正された。エージェントのプロンプトとツール制限が復元されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークツリー分離サブエージェントのgitリダイレクト修正

ワークツリー分離されたサブエージェントが`git -C`、`--git-dir`、または`GIT_DIR`/`GIT_WORK_TREE`経由で共有チェックアウトにgitをリダイレクトしていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークツリーセッションのディレクトリ不一致修正

作業ディレクトリが選択されたプロジェクトと一致しない場合に、別のプロジェクトの残留ワークツリーに着地していた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## gitリポジトリなしのバックグラウンドセッション削除修正

ワークツリーにgitリポジトリがないバックグラウンドセッションが削除できなかった問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude daemon stop --any`のプロセス終了修正

古いレガシーデーモンのロックファイルにより、無関係のプロセスを終了させる可能性があった問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Esc-Escでのリワインドピッカー表示修正

バックグラウンドタスクがある長時間実行セッションで、アイドルプロンプト時のEsc-Escがリワインドピッカーを開かなかった問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bashコマンドの権限チェック修正

`&&`リストや否定内のリダイレクト付き複合文に対するBashコマンドの権限チェックが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)
