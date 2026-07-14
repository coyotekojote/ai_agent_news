## GitHub MCPツールセット設定の永続化

GitHub MCPツールセット/ツール設定（githubMcpToolsets、githubMcpToolsなど）がsettings.jsonに永続化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## プラグインマーケットプレイスサブコマンドの追加

プラグインマーケットプレイスの一覧表示、追加、削除を行う`plugins marketplace`サブコマンドが追加された。また、プラグインマーケットプレイスの閲覧・更新コマンドも追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## サイドバーセッションの再起動後の永続化

サイドバーセッションが再起動後も永続化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## /worktreeと/moveの分離

`/worktree`と`/move`が分離された。`/worktree`は新しいワークツリーを作成しコミットされていない変更を残し、新しい`/move`はそれらをワークツリーに持ち込むようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## /chronicleへのローカル・クラウドコストプロファイル追加

`/chronicle`のcost-tipsにローカルおよびクラウドのコストプロファイルが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## モデルピッカーのAuto説明表示改善

モデルピッカーがAutoモデルの説明をクリック可能なLearn Moreリンク付きのMarkdownとして表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## セッションの作業ディレクトリ維持

セッションがプロンプト、再起動、ワークスペースツール間で作業ディレクトリに紐付けられ維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## ask_userチョイスプロンプトのカスタム回答拡張

ask_userチョイスプロンプトでカスタム回答の利用範囲が拡張された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## サブエージェントのネスト深度制限変更

デフォルトの最大サブエージェントネスト深度が6から4に削減された。使用量ベース課金ユーザーは最大128まで調整可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## Autopilotのターン中切り替え時の自動回答

Autopilotのターン中切り替え時に、そのターン中に提示された質問に自動回答するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## カスタムエージェントのシェルツール要求修正

シェルツールをエイリアスで要求するカスタムエージェントが、一致するread、list、stopシェルツールも受け取るようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## スラッシュコマンドの大文字小文字区別の廃止

スラッシュコマンドとオートコンプリートが大文字小文字を区別しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## Repo有効化プラグインの表示修正

Repo有効化プラグインが`/plugin`リストおよびスキルピッカーに表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## クイックヘルプの二重?キー押下動作修正

?を二重押しでクイックヘルプが閉じ、リテラルの?でプロンプトを開始できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## シェル補完の位置引数チョイス提案

シェル補完が位置引数のチョイスを提案するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## Linuxでの/appの起動メッセージ即時表示

`/app`の起動メッセージとダウンロードリンクがLinuxで即座に表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## --max-autopilot-continuesのバリデーション強化

`--max-autopilot-continues`がNaN、負の値、小数値を拒否するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## NO_COLOR環境変数の対応

CLIでNO_COLOR環境変数が尊重されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## /settings変更後のセッションオプション即時更新

`/settings`変更後にセッションオプションが即座に更新されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## /modelおよびピッカー行のスクリーンリーダー対応

`/model`およびピッカー行にフォーカスした際のスクリーンリーダーアナウンスが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## カスタムエージェントの重複表示修正

カスタムエージェントが`/agent`で一度だけ表示され、ソースラベルが保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## /model料金バナーのクリア修正

モデルが一致しない場合に`/model`の料金バナーがクリアされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## /shareのファイル出力パス修正

`/share file session`および`/share html session`の出力パス処理が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## --contextの新規対話セッション対応

`--context`が新規の対話セッションで尊重されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## モデルピッカーの隠しモデル設定変更防止

モデルピッカーが空の検索時に隠しモデル設定を変更しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## プラグインルートスキルの表示修正

プラグインルートスキルが`/plugin:plugin`ではなく`/plugin`として表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## フックエントリの不正時の有効フック保持

単一のフックエントリが不正な場合でも有効なフックが保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## write(path)拒否の指定パス限定

`write(path)`の拒否が指定されたパスのみをブロックするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## --add-github-mcp-toolのワイルドカード対応

`--add-github-mcp-tool "*"`ですべてのGitHub MCPツールが有効化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## 空の未追跡ファイルの表示修正

空の未追跡ファイルが擬似的な追加行なしでレンダリングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## copilot skill add失敗時のエラーメッセージ改善

copilot skill add失敗時にクリーンな失敗メッセージが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## 設定配列の空白アイテム処理改善

設定配列の空白アイテムの処理が改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## ブールトグルの登録デフォルト値対応

登録されたデフォルト値に対するブールトグルの動作が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## /cwdフォルダ信頼拒否時のセッション維持

`/cwd`のフォルダ信頼を拒否した際にライブセッションが維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## ワークスペースMCP設定の不正形式警告

ワークスペースMCP設定の不正形式時に警告が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## copilot mcpおよびcopilot skillのヘルプ表示

引数なしの`copilot mcp`および`copilot skill`がヘルプを表示して終了コード0で終了するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## allowed_models.txtの不正形式エラー表示

不正な形式の`allowed_models.txt`ポリシーエラーがクリーンに表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## 同期セッションの名前による再開修正

同期されたセッションの名前による再開が誤マッチなく機能するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## --nameと--session-idの既存セッションエラーメッセージ

既存セッションに対する`--name`と`--session-id`のエラーメッセージが改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## --plugin-dirプラグインのリスト表示

`--plugin-dir`プラグインが`copilot plugin list`に表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## バックグラウンドセッションのナビゲーション後の永続化

バックグラウンドセッションがナビゲーション後も永続化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## -p --stream offでの#number GitHubリファレンスリンク

`-p --stream off`出力で単独の#numberのGitHubリファレンスがリンクされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## 起動バナーのonce設定時の初回のみ表示

起動バナーがonce設定時に初回起動時のみ表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## copilot updateのstableチャンネル対応

`copilot update`および`/update`がチャンネルとして`stable`を受け付けるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## --plugin-dir警告のターミナル表示

`--plugin-dir`の警告がターミナルに表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## カスタムエージェント読み込みエラーの適切な報告

カスタムエージェントの読み込みエラーが適切に報告されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## --continueと--resumeの併用拒否

`--continue`が`--resume`との併用時に拒否されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## プロンプトモードの--shareエクスポート失敗時の終了コード修正

プロンプトモードが`--share`または`--share-gist`のエクスポート失敗時にゼロ以外の終了コードで終了するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## サーバーモードのOAuth MCPサーバー再接続

サーバーモードがキャッシュされたトークンからOAuth MCPサーバーに再接続するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)

## マーケットプレイスプラグインインストール時のGit認証ヘルパー維持

マーケットプレイスプラグインのインストール時にGit認証ヘルパーが利用可能な状態で維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71-1)
