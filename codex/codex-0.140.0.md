## /usageコマンドの追加

日別、週別、累積のアカウントトークン使用状況を表示する`/usage`ビューが追加された。

[参考リンク](https://github.com/openai/codex/pull/27925)

## /goalのリモートセッション対応強化

`/goal`がリモートセッションで大きなテキスト、大量のペーストブロック、画像添付を保持できるようになった。

[参考リンク](https://github.com/openai/codex/pull/27508)

## セッションの永久削除機能

`codex delete`、`/delete`、app-serverの`thread/delete` APIによる永久的なセッション削除が実装された。確認セーフガード付き。

[参考リンク](https://github.com/openai/codex/pull/25018)

## /importコマンドの追加

Claude Codeからセットアップ、プロジェクト設定、最近のチャットを選択的にインポートする`/import`コマンドが追加された。

[参考リンク](https://github.com/openai/codex/pull/27070)

## 統合メンションメニュー

`@`入力で、ファイル、プラグイン、スキルの統合メンションメニューがデフォルトで開くようになった。

[参考リンク](https://github.com/openai/codex/pull/27499)

## Amazon Bedrock API認証とOAuthクレデンシャル管理

マネージドAmazon Bedrock APIキー認証が追加された。CLIおよびMCP OAuthクレデンシャルの暗号化ローカルストレージも実装された。

[参考リンク](https://github.com/openai/codex/pull/27443)

## SQLiteデータベースの自動復旧

破損したSQLiteステートデータベースが自動的にバックアップされ、ロールアウトデータから再構築されるようになった。

[参考リンク](https://github.com/openai/codex/pull/26859)

## /reviewのクラッシュ修正

キューされたガイダンスがある状態でEscを押した際の`/review`クラッシュが修正された。レビューがキャンセルされた場合もガイダンスが保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/22879)

## MCP信頼性の向上

一時的な起動失敗がリトライされるようになり、使用不可なOAuthがログアウト状態として報告され、無効化されたサーバーが保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/25147)

## プラグイン管理の修正

リモートプラグインのアンインストールが修正され、インストール時に認証要件が表示されるようになった。

[参考リンク](https://github.com/openai/codex/pull/27085)

## 状態永続化の改善

「再度表示しない」の却下が確実に永続化され、ターン終了後に古い実行中フックインジケーターがクリアされるようになった。

[参考リンク](https://github.com/openai/codex/pull/27619)

## バックグラウンドコマンドの割り込み対応

非TTYバックグラウンドコマンドが出力と終了ステータスを保持しつつCtrl-Cで割り込み可能になった。

[参考リンク](https://github.com/openai/codex/pull/26734)

## 大規模リポジトリでのパフォーマンス改善

Gitの組み込みファイルシステムモニターが保持され、重複履歴読み取りの排除、アーカイブ検索の高速化、ターン差分レンダリングのキャッシュにより応答性が向上した。

[参考リンク](https://github.com/openai/codex/pull/26880)

## /realtimeボイスコントロールの削除

実験的な`/realtime`ボイスコントロールと関連オーディオ依存がTUIから削除された。

[参考リンク](https://github.com/openai/codex/pull/27801)
