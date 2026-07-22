## コードレビューのバックグラウンドサブエージェント化

`/code-review`がバックグラウンドサブエージェントとして実行されるようになり、会話がクリーンに保たれるようになった。レビュー作業が会話を埋め尽くさなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スクリーンリーダーの削除テキスト読み上げ対応

`--ax-screen-reader`モードで削除されたテキストのスクリーンリーダーアナウンスが追加された。`Option+Delete`、`Ctrl+W`、`Cmd+Backspace`、`Ctrl+U`、`Ctrl+K`の削除ショートカットがサポートされている。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windowsパスの`\u`プレフィックス破損修正

`\u`プレフィックスのセグメントを含むWindowsパス（例：`C:\Users\unicorn`）が破損し、CJK文字に変換されてファイルにアクセスできなくなる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッション管理の改善

左矢印キーで会話を破棄する前に確認が必要になった。エージェントビューで`Esc`キーを押すと、会話を失うのではなくバックグラウンドの会話に戻るようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPサーバー接続エラーの表示改善

`claude mcp list`および`/mcp`でサーバー接続失敗時にHTTPステータスとエラーテキストが表示されるようになった。また、MCP設定値に隠れた先頭/末尾の空白がある場合の警告が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ターミナル入力の改行処理修正

貼り付けた改行をCtrl+Jとしてエンコードするターミナルで、複数行の貼り付けが`j`で改行を置き換えて単一行に折りたたまれる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/context`のトークン使用量表示修正

メッセージコンパクション後に`/context`が古いトークン使用量を報告する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/ultrareview`の引数処理修正

`/ultrareview`が「review my auth changes」のような記述的な引数で失敗する問題が修正された。また、`/code-review ultra`が非インタラクティブセッションでローカルレビューをサイレントに実行する問題も修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ゲートウェイ課金のBedrock ARN価格設定修正

ゲートウェイの支出計測がBedrock application-inference-profile ARNを適切に価格設定するよう修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 絵文字切り詰め時の文字化け修正

長いIDE選択が絵文字の途中で切り詰められた際の文字化け（mojibake）が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サイレントツールエグゼキュータエラーの修正

サイレントツールエグゼキュータのエラーがドロップされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エンジンティアダウンの競合状態修正

エンジンのティアダウン競合によりファントムターンが発生する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 中断されたツールコール後の誤メッセージ修正

中断されたツールコール後に偽の「[Request interrupted by user]」メッセージが表示される問題が修正された。レスポンス途中でツールが中断された際にトランスクリプトで`tool_use`ブロックが対になっていない問題も修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スクリーンリーダーのスペース入力読み上げ修正

`--ax-screen-reader`モードでVoiceOverがスペース入力時に「new line」と読み上げる問題が修正された。プラグインおよび設定パネルでスクリーンリーダー/拡大鏡向けにフォーカス行にカーソルが移動しない問題も修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 深くネストされたディレクトリツリーのクラッシュ修正

深くネストされた監視ディレクトリツリーによるクラッシュ（maximum call stack exceeded）および深くネストされたUIツリーのレンダリング時のクラッシュが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プルリクエストイベントのセッション終了時損失修正

セッション終了時にプルリクエストイベントが時折失われる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrockセットアップウィザードのプロファイル検証修正

Bedrockセットアップウィザードがパーティション分割されたAWSリージョンのassume-roleプロファイルの検証に失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## モノトニッククロックによるターン時間計測修正

システムクロック調整後にまれに負の値や不正確なターン時間が計測される問題が修正され、モノトニッククロックが使用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude.aiのMCPサーバー認証カウント修正

claude.aiで「N MCP servers need authentication」の通知が過剰にカウントされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プロンプト履歴の書き込み競合修正

書き込みが競合またが失敗した際にプロンプト履歴エントリがドロップまたは重複する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## コンテキストオーバーフロー後のリトライループ修正

コンテキストオーバーフローエラー後にリトライループが失敗確定のリクエストを再送信する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントフロントマターフックのセキュリティ強化

信頼されていないフォルダからエージェントフロントマターフックが実行される問題が修正された。フックはそのフォルダに対するワークスペース信頼を要求するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フォークセッション系譜のコンパクション修正

ヘッドレス/SDKセッションでコンパクション後にフォークセッションの系譜が失われる問題が修正された。不正なデルタ添付によりレジュームセッションが失敗/クラッシュする問題も修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 自動モード分類器の改善

dangerous-rm、バックグラウンド`&`、疑わしいWindowsパスのチェックが権限ダイアログを開かなくなった。自動モード分類器がこれらの判断を行うようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/deep-research`の手動起動化

`/deep-research`が手動で呼び出された場合のみ開始されるようになった。Claudeが自動的に起動しなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プランモードでの自動モード改善

プランモードで自動モードがBashの読み取り専用コマンドに対してプロンプトを表示しなくなった。自動モード分類器が判断するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ファストモード切り替えのアナウンス追加

`/config model=<x>`またはRemote Controlによりファストモードが変更された際のアナウンスが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サーバー管理設定の承認プロンプト変更

無害な機能やコストのトグルに対するサーバー管理設定が承認プロンプトをトリガーしなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェント名のコロン禁止

エージェントマークダウンファイルで`:`を含むエージェント名が拒否されるようになった。プラグインの名前空間用に予約された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スキルの`context: fork`バックグラウンド実行

`context: fork`を持つスキルがデフォルトでバックグラウンドで実行されるようになった。スキルごとに`background: false`でオプトアウトできる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フロントマターブーリアン値の拡張

スキルおよびプラグインのフロントマターブーリアンで`yes`/`no`/`on`/`off`/`1`/`0`（大文字小文字不問）が受け入れられるようになった。既存の`true`/`false`に加えてサポートされた。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リモートセッションのハートビート修正

ワーカー置換後もリモートセッションがハートビートを送信し続け、デスクトップ/IDEプロセスが拒否されたリクエストを無期限にリトライする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)
