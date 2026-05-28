## Opus 4.8対応

Opus 4.8がデフォルトモデルとなり、最も困難なタスクに対して高エフォート（`/effort xhigh`）がデフォルトで適用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ダイナミックワークフロー

Claudeにワークフローの作成を依頼すると、バックグラウンドで数十から数百のエージェントを協調させて作業を実行する。`/workflows`で実行状況を確認可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ファストモード料金改定

Opus 4.8のファストモードが標準料金の2倍で2.5倍の速度で利用可能になった（以前のコストの一部）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## システムプロンプト・エフォート改善

リーンシステムプロンプトがHaiku、Sonnet、Opus 4.7以前を除く全モデルでデフォルトになった。Claudeが自ら判断できない場合のみ多肢選択プロンプトを使用するようになった。`/effort`スライダーのラベルが「Speed」/「Intelligence」から「Faster」/「Smarter」に変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /simplifyコマンドの変更

`/simplify`がバグハンティングレビューではなくクリーンアップ専用レビュー（再利用、簡略化、効率性、アルティチュード）を実行し修正を適用するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsのシェルコマンド対応

`! <command>`でシェルコマンドをバックグラウンドセッションとして実行し、アタッチ・デタッチが可能になった。`claude --bg --exec '<command>'`としても利用可能。`/logout`がバックグラウンドセッションへの送信ではなくサインアウトを実行するようになった。`←←`によるエージェントビュー表示がBedrock、Vertex、Foundry、テレメトリ無効時にも対応。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Chrome連携の強化

`/chrome`→「Select browser…」で接続中のブラウザを選択可能になった。複数ブラウザ接続時にチャット内でブラウザアクション実行時にも選択可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグイン制御・発見の改善

プラグインが`plugin.json`またはマーケットプレイスエントリで`defaultEnabled: false`を宣言可能になった。`/plugin`のDiscoverタブがカレントディレクトリに関連するプラグインを「suggested for this directory」と注釈付きでピン留めするようになった。有効化されたプラグインの依存関係が自動で有効化されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ストリーミング・MCP改善

ストリーミングツール実行がテレメトリ無効時やBedrock/Vertex/Foundry上でも常に有効になった。stdio MCPサーバーサブプロセスに`CLAUDE_CODE_SESSION_ID`と`CLAUDECODE=1`環境変数が渡されるようになった。`claude mcp list`/`get`で未承認の`.mcp.json`サーバーが自動承認される代わりに`⏸ Pending approval`と表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セキュリティ改善

データ流出（特にリポジトリの一括転送）に対するAutoモード分類器の検出が改善された。`HOME`に末尾スラッシュがある場合の`rm -rf $HOME`ブロック漏れが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

`$TMPDIR`の解決先不一致、`claude agents`のテーマ不一致時のテキスト可読性、1Mコンテキストモデルでのバックグラウンドエージェント完了通知の誤動作、バックグラウンドセッション分類器のゴール喪失、ピン留めバックグラウンドセッションの再生成ループ、`worktree.baseRef: "head"`の解決先誤り、VS Codeでのターミナルレンダリング破損、Autoモードでの安全性分類器のトークン超過時の誤ブロック、Windowsの更新失敗時エラー表示など多数の問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)
