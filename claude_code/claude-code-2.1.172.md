## ネストされたサブエージェント（最大5階層）

サブエージェントが自身のサブエージェントを起動できるようになり、最大5階層までの階層的なエージェントワークフローが可能になった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## Amazon BedrockのAWSリージョン検出の改善

`AWS_REGION`環境変数が設定されていない場合、Amazon Bedrockが`~/.aws`設定ファイルからリージョンを読み取るようになった。AWS SDKの優先順位規則に準拠する。`/status`コマンドでリージョンの取得元が表示される。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## プラグインマーケットプレイスへの検索バー追加

`/plugin`マーケットプレイスでプラグインを閲覧する際に検索バーが追加され、プラグインの発見性が向上した。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## OTELメトリクスへのモデル属性追加

`claude_code.lines_of_code.count` OTELメトリクスに`model`属性が追加され、使用モデル別のコードメトリクスの追跡やフィルタリングが可能になった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## 1Mコンテキストセッションのスタック修正

使用クレジットなしで1Mコンテキストを使用しているセッションが永続的にスタックする問題が修正された。標準コンテキスト制限以下に自動的にコンパクトされるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## 画像処理エラーの修正

会話に複数の画像が含まれている場合に「画像を処理できませんでした」というエラーが繰り返し表示される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## エージェントビューのスピナー表示修正

ワーカーが応答した後もセッションが最大30秒間「Working」ステータスのままビジースピナーが表示され続ける問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## バックグラウンドエージェントのディレクトリ分離修正

プリウォームされたワーカーにディスパッチされた際に、バックグラウンドエージェントが別ディレクトリのプロジェクト設定（`.mcp.json`の承認やトラスト）を読み込む可能性がある問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## サブエージェントのスタック状態修正

ネストされたエージェントが停止された後もバックグラウンドサブエージェントがエージェントパネルで「active」のままスタックする問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## availableModels制限の適用範囲拡大

`availableModels`の制限がサブエージェントのモデルオーバーライド、エージェントディスパッチのモデルピッカー、アドバイザーモデルに適用されていなかった問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## モデルIDの1Mサフィックス重複修正

`ANTHROPIC_DEFAULT_OPUS_MODEL`に既に1Mサフィックスが含まれている場合、モデルIDが二重の1Mコンテキストサフィックス（例：`[1M][1m]`）になる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## WebFetchワイルドカードドメインの修正

`WebFetch(domain:*.example.com)`のワイルドカードパターンがallow/deny/askルールでサブドメインにマッチしない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## ファイルパーミッションのワイルドカード修正

パターン中間のワイルドカード（例：`Read(secrets-*/config.json)`）を含むファイルパーミッションルールが起動時に拒否される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## チームメモリストアの修正

リモートセッションでマウントされたチームメモリストア（`CLAUDE_MEMORY_STORES`）がメモリリコールで検出されない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## ワークフローバリデーションの修正

プロンプト文字列やコメントに`Date.now()`や`Math.random()`が含まれるだけでワークフローバリデーションがスクリプトを拒否する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## 長い会話でのパフォーマンス改善

冗長なメッセージ正規化の削除、ストリーミングツール使用状態が変更されていない場合のメッセージ履歴全体の変換回避、`/goal`ステータスチップのアイドル時5Hz再レンダリングの削減、サブエージェント並列実行時のUI再レンダリング削減によりパフォーマンスが改善された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## バックグラウンドセッションアタッチの修正

デーモン自動更新後に古いバージョンで開始されたセッションにアタッチする際のEAUTHエラーが修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## Windows・VSCode関連の修正

Windowsコンソールでマウストラッキングが完全にサポートされていない場合に無効化されるようになった。VSCodeでPowerShellツールコールが適切なコマンド表示とパーミッションダイアログの代わりに生のJSONとしてレンダリングされる問題が修正された。VSCodeの表示シェル出力からANSIエスケープコードが除去されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)

## Chrome統合ツール読み込みの改善

ブラウザツールがツールごとの個別呼び出しではなく、単一のバッチ呼び出しで読み込まれるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.172)
