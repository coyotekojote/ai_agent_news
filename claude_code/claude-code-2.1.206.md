## /cdコマンドへのディレクトリパスサジェスト追加

`/cd`コマンドに`/add-dir`と同様のディレクトリパスサジェストが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /doctorによるCLAUDE.mdファイルのトリミング提案

`/doctor`チェックにおいて、Claudeがコードベースから導出可能な内容を含むチェックイン済み`CLAUDE.md`ファイルのトリミングを提案する機能が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /commit-push-prのgit push自動許可拡張

`/commit-push-pr`がリポジトリに設定されたプッシュリモート（`remote.pushDefault`、またはリモートが1つのみの場合はそのリモート）への`git push`を`origin`に加えて自動許可するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Gateway: /loginのAnthropicパブリックゲートウェイ対応

`/login`がAnthropic運営のパブリックゲートウェイエンドポイントをサポートするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## EnterWorktreeの確認ダイアログ追加

`EnterWorktree`がプロジェクトの`.claude/worktrees/`ディレクトリ外のgitワークツリーに入る前に確認を求めるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントのバージョンアップグレード改善

バックグラウンドエージェントがClaude Codeアップデート直後にバックグラウンドで新バージョンにアップグレードするようになり、アタッチ時の遅いアップグレードが不要になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 期限切れログインのエラーメッセージ修正

期限切れのログインが「There's an issue with the selected model」という誤解を招くエラーを表示する代わりに、`/login`の実行を促すようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude --resumeおよび--continueの起動時入力修正

`claude --resume`および`--continue`が起動時にキーボード入力に応答しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPサーバーのrequest_timeout_ms無視修正

`--mcp-config`または`.mcp.json`で設定されたMCPサーバーがサーバーごとの`request_timeout_ms`を無視し、新規セッションで60秒のデフォルトタイムアウトが適用される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## CLAUDE_CODE_EXTRA_BODYのバックグラウンドワーカー対応修正

`CLAUDE_CODE_EXTRA_BODY`が`claude agents`/`--bg`バックグラウンドワーカーで無視される問題が修正され、シェルでエクスポートされたオーバーライドがディスパッチセッションに引き継がれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OAuth MCPサーバーの再認証修正

OAuth MCPサーバーが単一のトークンリフレッシュ失敗後に手動再認証を必要とする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## --permission-prompt-toolのMCPサーバー起動時クラッシュ修正

`--permission-prompt-tool`がMCPサーバーを指している場合、サーバー接続完了前にコールドスタートで「MCP tool not found」クラッシュが発生する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /modelピッカーの価格表示修正

`/model`ピッカーの行が名前とは異なるモデルの価格を表示する問題が修正され、プロバイダーが請求しないファーストパーティ定価の引用が停止された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /modelピッカーのモデル行配置修正

サーバー提供のモデル行が、エンタイトルメントまたは許可リスト制限によって配置対象の行が削除された場合に`/model`ピッカーで誤った位置に表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## デスクトップセッションのスラッシュコマンド送信後のスタック修正

スラッシュコマンドがターン中に送信された後、デスクトップセッションが「running」表示のまま停止する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windows上のclaude --resumeのキーボード入力修正

Windowsでベアの`claude --resume`の前にセットアッププロンプトが表示された際にエージェントビューでキーボード入力が無視される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude rmのデーモンロスター残留修正

`claude rm`が削除されたジョブをデーモンロスターに残し、`claude agents`で行が再表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /remote-controlのログアウト時エラー修正

`/remote-control`がログアウト時に「Unknown command」を表示する代わりに、サインイン方法を説明するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフロー詳細ビューの左矢印ナビゲーション修正

ワークフロー詳細ビューでフェーズまたはエージェントから戻る際に左矢印キーが機能しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /statusの重複警告修正

`/status`が同じインストール破損警告を2回表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## LSPプラグインの誤った未使用判定修正

LSPプラグインに対する誤った「disused plugin」ヒントと不正確な未使用テレメトリが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /doctorのアップデートチェック修正

`/doctor`のアップデートチェックがHomebrewインストールに対して設定チャネルではなくcaskのチャネルと比較するように修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フルスクリーンのジャンプトゥボトムピル修正

フルスクリーンのジャンプトゥボトムピルがmacOSでCtrl+Endを提案する問題、リバウンドされたコードの非表示、トランスクリプト上への折り返しが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrock: 起動ハング修正

制限されたエグレスのネットワークで`awsCredentialExport`ヘルパーを使用する際にBedrock環境で数分間の起動ハングが発生する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /code-reviewの品質改善

claude-opus-4-8でのすべてのエフォートレベルにおける`/code-review`の検出品質が改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューのステータス列幅改善

エージェントビューのステータス列が64文字で切り詰められるのではなく、ターミナル全幅を使用するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューのCtrl+Xによるセッション削除

エージェントビューでCtrl+Xが完了済みセッションを永久に削除するようになり、セッションの二重レンダリングが解消された。削除されたバックグラウンドジョブは削除状態が維持される。

[参考リンク](https://code.claude.com/docs/en/changelog)
