## ワークツリー分離セッションのセキュリティ修正

ワークツリー分離セッションおよびそのサブエージェントがメインチェックアウトに対して破壊的なgitコマンドを実行できる問題が修正された。すべてのセッションタイプでファイル編集とBashに分離が適用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PreToolUseフックのセキュリティ修正

PreToolUse自動許可フックがバックグラウンドエージェントタスク（サマリー、コンパクション、リネーム）のツール制限をバイパスする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 利用クレジットリクエストの修正

TeamおよびEnterpriseで`/usage-credits`を実行した際に「利用クレジットリクエストを既に送信済み」と表示される問題が修正された。以前のリクエストが却下されたメンバーが新しいリクエストを送信できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スタートアップ接続チェックの修正

HTTPSプロキシ背後でスタートアップ接続チェックがハングしてから失敗する問題が修正された。APIリクエストと同じプロキシ対応トランスポートを使用し、明確なメッセージでタイムアウトするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 「接続がレスポンス途中で切断」エラーの修正

実際には完了していたレスポンスに対して「Connection closed mid-response」エラーが誤って報告される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/usage`のMCPサーバー使用量の修正

`/usage`がMCPサーバーへの使用量を過大に帰属させる問題が修正された。サーバーのシェアがそのツール結果を消費したリクエストのみを反映するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PRリンクの修正

ブランチがプッシュされた後に作成されたプルリクエストにセッションがリンクされない問題が修正された。GitHub REST API経由の場合も含む。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 組織制限モデルエイリアスの修正

組織制限付きの`model: opus`スタイルのサブエージェントおよびチームメイトのファミリーエイリアスが修正された。親モデルにドロップする代わりに、ファミリー内の最新の組織許可モデルにステップダウンするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ストリームアイドルタイムアウトの修正

カスタム`ANTHROPIC_BASE_URL`ゲートウェイでサーバーキープアライブピンが到着しているにもかかわらずストリームアイドルタイムアウトが発火する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude.aiコネクタの認証状態修正

claude.aiコネクタが誤って認証が必要とマークされる問題が修正された。無効なセッショントークンでは`/login`ヒントが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ツールエラー表示の修正

ローカルで利用不可になったツール（例：MCPサーバーが削除された場合）のツールエラーが表示されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## SendMessageの長いサマリー修正

`SendMessage`が長いサマリーを拒否する問題が修正された。送信が文字数制限で失敗する代わりにトランケートされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントのeffortラベル修正

サブエージェントのトランスクリプトビューでスピナーのeffortラベルがサブエージェント自身の`effort:`設定ではなくセッションのeffortレベルを表示していた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ファイルウォッチャーのクラッシュ修正

ファイルウォッチャーがファイルシステムエラーに遭遇した場合、またはファイルウォッチャーのティアダウン中にまれにクラッシュする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スクリーンリーダーのバックスペース修正

`--ax-screen-reader`モードでバックスペースのたびにスクリーンリーダーが入力行全体を再読み上げする問題が修正された。行末の削除では削除された文字のみがエコーされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ホストモデル選択キーの修正

`CLAUDE_CODE_PROVIDER_MANAGED_BY_HOST`が設定されている場合に、古いディスク上の`managed-settings.json`よりもホストのモデル選択キーが優先されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## オートモードの安全性向上

`SendMessage`経由で他のエージェントセッションに送信されるメッセージが、ディスパッチ前に権限分類器によって評価されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スキル呼び出し拒否の改善

`disable-model-invocation`が設定されたスキルをClaudeが呼び出そうとした際の拒否メッセージが改善された。ワークフローを再現する代わりに、ユーザーにスキルの実行を依頼するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## diffビューの改善

`/diff`ビュー、Remote Controlワークスペースdiff、およびファイル編集diffが改善された。Claude Code on webセッションで、ワークスペースに設定されたdiffドライバーやtextconvを無視してrawのgit blobコンテンツを使用するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Control自動起動の変更

リポジトリローカル設定（`.claude/settings.json`または`.claude/settings.local.json`）からRemote Controlをオンにできなくなった（オフにすることは引き続き可能）。ユーザースコープで`/config`から有効化する必要がある。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ultraplan機能の削除

ultraplan機能が削除された。

[参考リンク](https://code.claude.com/docs/en/changelog)
