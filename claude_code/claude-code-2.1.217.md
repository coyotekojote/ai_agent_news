## 絵文字ショートコードのオートコンプリート

プロンプト入力で絵文字ショートコードのオートコンプリートが追加された。`:heart:`と入力すると❤️が挿入され、`:hea`で候補が表示される。`emojiCompletionEnabled`設定で無効化できる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## トランスクリプト書き込み失敗時の警告表示

トランスクリプト書き込みが失敗している場合（ディスク容量不足など）や、継承された環境変数によりセッション保存がオフになっている場合に警告が表示されるようになった。トランスクリプトが無言で失われることが防止された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPツール出力のメモリリーク修正

切り詰められたMCPツール出力が、セッションの残りの間、完全な未切り詰め結果をメモリに保持していたメモリリークが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windows自動更新失敗時の実行ファイル復元

自動更新の失敗により`claude.exe`が消失する可能性があったWindows上の問題が修正された。更新が失敗した場合、保存された実行ファイルが自動的に復元される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッション分離のシンボリックリンク正規化修正

バックグラウンドセッション分離がシンボリックリンクされた作業ディレクトリを正規化しておらず、セッションがワークスペースフォルダから脱出できていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrock上のClaude Opus 4.8の自動コンパクト修正

Bedrock上のClaude Opus 4.8で自動コンパクトがトリガーされない問題と、制限を超えた後に`/compact`が失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 企業向けmTLS/プロキシ設定の修正

企業向けmTLS、TLS検証、OAuthスコープ、プロキシ設定がClaude Desktopセッションで無視されていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スクリーンリーダーモードの修正

スクリーンリーダーモードの起動アナウンスが最初のプロンプトレンダリングで切り取られる問題と、思考ステータス行が経過時間とトークンカウントを更新するために数秒ごとに再レンダリングされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 管理設定のOTELエンドポイント制御修正

`OTEL_EXPORTER_OTLP_ENDPOINT`を設定する管理設定がすべてのシグナルを制御しない問題が修正された。より低いスコープのシグナル固有のオーバーライドがテレメトリを管理エンドポイントからリダイレクトしなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `--resume`/`--continue`のTypeError修正

トランスクリプトに不正な添付エントリがある場合に、`--resume`/`--continue`および`/resume`がTypeErrorで失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リモートコントロールの権限プロンプト表示修正

リモートコントロールセッションで、権限プロンプトやダイアログが表示された後に接続したビューアに保留中のプロンプトが表示されなかった問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドシェルの停止不能問題の修正

セッションがバックグラウンドに送信された後（`/background`または`←`）、またはセッション終了時にバックグラウンドシェルが停止不可能になることがあった問題が修正された。特にWindows上で顕著だった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## CLAUDE.md/SKILL.mdのブレース展開によるOOM修正

`CLAUDE.md`や`SKILL.md`のpathsフロントマターの値に多数のブレースグループがある場合にCLIが起動時にOOMキルまたはストールする問題が修正された。ブレース展開にバジェット制限が設けられた。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッション接続時のトランスクリプトプレビュー修正

起動中のバックグラウンドセッションに接続する際に、トランスクリプトプレビューが入力エリアに密着していた問題が修正された。ライブレイアウトと同じ1行のギャップが設けられるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PRバッジリンクのクリック可能化

フッターのPRバッジリンクが、ターミナルサポートが検出できない場合（ssh/tmux経由など）でもクリック可能なハイパーリンクとして表示されるようになった。`FORCE_HYPERLINK=0`でオプトアウトできる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ログイン期限切れ警告の変更

ログイン期限切れの警告が、期限切れの5日前から3日前に変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フロントエンドデザインプラグイン提案の表示制限

フロントエンドデザインプラグインの提案ティップが、無制限に繰り返し表示されるのではなく、生涯3回に制限された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 同時実行サブエージェント数の上限追加

同時実行サブエージェントに上限が設けられた（デフォルト20、`CLAUDE_CODE_MAX_CONCURRENT_SUBAGENTS`でオーバーライド可能）。1つのメッセージが無制限にバックグラウンドエージェントを展開できなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントのネスト制限

サブエージェントがデフォルトでネストされたサブエージェントを生成しなくなった。`CLAUDE_CODE_MAX_SUBAGENT_SPAWN_DEPTH`を設定することでより深いネストを許可できる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `--max-budget-usd`のバックグラウンドサブエージェント停止修正

`--max-budget-usd`がバックグラウンドサブエージェントを停止しなかった問題が修正された。上限に達すると新しいスポーンが拒否され、実行中のバックグラウンドエージェントが停止されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)
