## Bedrock・Vertex AI・Foundryでのオートモード一般提供

オートモードが`CLAUDE_CODE_ENABLE_AUTO_MODE`のオプトインなしでBedrock、Vertex AI、Foundryで利用可能になった。`disableAutoMode`設定で無効化可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrock・Vertex・Claude Platform on AWSのデフォルトモデル変更

Bedrock、Vertex、Claude Platform on AWSのデフォルトモデルがClaude Opus 4.8に変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ストリーミング中の長大コンテンツによるターミナルフリーズ修正

非常に長いリスト、テーブル、段落、コードブロックを含むレスポンスのストリーミング中にターミナルがフリーズしキーストロークが遅延する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 非対話実行時のリモート管理設定の同意記録修正

非対話実行（`claude -p`、SDK）からのリモート管理設定がセキュリティ同意ダイアログを表示せずに恒久的に同意済みとして記録される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プロンプトインジェクション誤警告の修正

無害なシステム生成の会話更新によってトリガーされる誤ったプロンプトインジェクション警告が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 自動アップデーターによるカスタムランチャースクリプト上書き修正

自動アップデーターがリリースごとに`~/.local/bin/claude`のカスタムランチャースクリプトまたはシンボリックリンクを上書きする問題が修正された。`/doctor`が外部管理ランチャーを報告するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## cdを含む複合コマンドのパーミッションプロンプト修正

出力リダイレクトが`/dev/null`のみの場合に`cd`を含む複合コマンドがパーミッションを要求する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## レスポンス完了時のトランスクリプトジャンプ修正

レスポンスのストリーミング完了時にトランスクリプトが回答の先頭より上にジャンプする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## worktreeConfig残留によるgo-gitツール破壊の修正

最後の`worktree.sparsePaths`ワークツリー削除後に`extensions.worktreeConfig`がリポジトリの`.git/config`に残り、go-gitツール（`tea`など）が破壊される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ルールグロブ・スキルパスの不正ブラケットパターン修正

ルールグロブ、スキルパス、`.ignore`、`.worktreeinclude`内の不正なブラケットパターンがファイル読み取り、ファイルサジェスト、ワークツリー作成を破壊する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントチームのメールボックスメッセージによるクラッシュループ修正

不正なチームメイトメールボックスメッセージがエージェントチームで毎秒エラーを繰り返すクラッシュループを引き起こし、メールボックスファイルの手動削除が必要になる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションのプラン承認時の名前表示修正

プラン承認で自動命名されたバックグラウンドセッションがエージェントビューの行にその名前を表示しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## gitワークツリーに入ったバックグラウンドセッションの再開修正

gitワークツリーに入ったバックグラウンドセッションがエージェントリストからのコールドリオープン後に空白で再開する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Controlのタスクステータス更新消失修正

ネットワーク中断またはクレデンシャルリフレッシュからの接続回復時にRemote Controlのタスクステータス更新が失われる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## デスクトップアプリのRemote Controlセッション進捗表示修正

デスクトップアプリがホストするRemote Controlセッションがモバイルおよびウェブでバックグラウンドエージェントとワークフローの進捗を表示しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Deep researchのFetchフェーズエージェントラベル修正

Deep researchの実行がすべてのFetchフェーズエージェントを「unknown」とラベル付けする問題が修正され、チップがソースホスト名を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## BedrockのAWS SSOクレデンシャル繰り返し要求修正

BedrockがIAM Identity Centerに対してAPIリクエストごとに新しいAWS SSOクレデンシャルを繰り返し要求する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューのペーストテキスト重複改善

同じテキストを再度ペーストした際に、折りたたまれた`[Pasted text #N]`プレースホルダーが展開されるようになり、2つ目が追加されなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ブロックされたセッションピークの表示改善

ブロックされたセッションピークが質問を先頭に表示し、同じタイムスタンプの2回表示の代わりにテキスト表記の経過時間（`waiting 3m`）を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## オートモードの設定読み込み変更

オートモードが`.claude/settings.local.json`（リポジトリ内）から`autoMode`を読み込まなくなった。代わりに`~/.claude/settings.json`を使用する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WindowsでのAWSクレデンシャル解決ハング修正

AWSクレデンシャル解決が停止した場合（例：停止した`credential_process`）にWindowsで無期限にハングする問題が修正され、60秒のストールガードが正常に作動するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインフック・モニターのシェルインジェクション修正

プラグインのフック・モニター・MCP headersHelperにおいて、シェル形式コマンド内の`${user_config.*}`が拒否されるようになった（シェルインジェクション修正）。フックはexec形式（`args`配列）または`$CLAUDE_PLUGIN_OPTION_<KEY>`の使用が必要。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインオプション値の読み込み元制限

プラグインオプション値（`pluginConfigs`）がプロジェクトレベルの`.claude/settings.json`から読み込まれなくなった。ユーザー設定、`--settings`、マネージド設定のみが使用される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /usage-creditsの入力値バリデーション強化

`/usage-credits`の金額入力が不正な値（ペーストされたタイムスタンプなど）を無言で数字に変換する問題が修正され、不正な金額はエラーで拒否されるようになった。$1,000を超える金額は確認入力が必要になった。

[参考リンク](https://code.claude.com/docs/en/changelog)
