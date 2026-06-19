## 自動モードの安全性改善

破壊的なgitコマンド（`git reset --hard`、`git checkout -- .`、`git clean -fd`、`git stash drop`）がユーザーの明示的な指示なしにブロックされるようになった。また、`git commit --amend` はそのセッションでエージェントが作成したコミット以外ではブロックされ、`terraform destroy`/`pulumi destroy`/`cdk destroy` も特定のスタック指定がない限りブロックされる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 非推奨モデル警告の追加

リクエストされたモデルが非推奨または自動更新された場合に警告が表示されるようになった。printモード（`-p`）ではstderrに出力され、エージェントフロントマターで設定されたモデルもカバーされる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `attribution.sessionUrl` 設定の追加

WebおよびRemote Controlセッションでコミットやプルリクエストからclaude.aiセッションリンクを省略するための `attribution.sessionUrl` 設定が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/config --help` の追加

`/config key=value` で利用可能な全ショートハンドキーを一覧表示する `/config --help` が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/config` トグル動作の変更

EnterとSpaceの両方で選択した設定を変更できるようになり、Escが元に戻すのではなく保存して閉じるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 起動時の「setup issues」行の削除

ロゴ下の起動時「setup issues」行が削除された。設定の問題を確認するには `/doctor` を実行するか `--debug` を使用する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントスポーン時の400エラー修正

特定の設定で `thinking.disabled.display: Extra inputs are not permitted` 400エラーがサブエージェントのスポーンやセッションタイトル生成時に発生する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントでのWebSearch空結果修正

サブエージェントでWebSearchが空の結果を返す問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## vimモードでのカーソル位置修正

ネイティブカーソル有効時にvimモードで履歴ナビゲーション後にターミナルカーソルがプロンプトの上に残る問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windows TerminalでのTUI表示崩れ修正

Windows Terminalでネストされたサブエージェントの高負荷時にフルスクリーンTUIの表示が崩れる問題（ステータスラインの画面中央表示、スピナー行の重複、テキストの結合）が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 思考ブロックのみのレスポンス修正

モデルが思考ブロックのみを返した場合にターンが無出力で完了する問題が修正され、Claudeが一度再プロンプトするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スキルの重複表示修正

複数のプラグインが有効な場合にユーザーレベルのスキルがスラッシュコマンドオートコンプリートに複数回表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ヘッドレス/SDKモードでのMCP認証スタブツール修正

認証が必要なMCPサーバーがヘッドレス/SDKモードで認証スタブツールをモデルに公開する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## tmuxチームメイトペーンの起動修正

シェルのrc初期化が遅い場合にtmuxチームメイトペーンの起動が失敗する問題と、エージェントスポーン中に入力したキーストロークがリーダープロンプトではなく新しいtmuxペーンに漏れる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## チームメイト終了時のバックグラウンドタスク修正

チームメイトがターンを完了した際に、チームメイトが開始したバックグラウンドタスクが終了される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スケジュールタスクとWebhookトリガーの入力分類修正

スケジュールされたタスクとWebhookトリガーの配信がキーボード入力として扱われる問題が修正され、タスク通知として分類されるようになった。自動モードで保留中のアクションを承認したりセッションタイトルを設定したりできなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フォーカスモードのPostToolUseフック表示修正

フォーカスモードで各レスポンスの下に「Ran N PostToolUse hooks」のタイミング行が表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)
