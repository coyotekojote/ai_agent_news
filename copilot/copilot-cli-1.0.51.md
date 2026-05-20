## セッション管理の--session-idパラメータ

`--session-id=<id>`パラメータが追加され、既知のタスクの再開や特定のUUIDでの新規セッション作成が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## リモートコマンドの組織ポリシー対応

リモートコマンドが「組織のリモートコントロールおよびクラウドからの表示ポリシー」を強制するようになり、無効時にはエラーメッセージが表示されるようになった。エージェントがアクティブに作業中でもリモートコマンドが利用可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## カスタマイズ可能なステータスライン

ターミナルフッターのステータスラインがカスタマイズ可能になり、モデル、コンテキストウィンドウ、gitブランチなどのセッション情報が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## MCPツール読み込みの高速化

起動時のMCPツール読み込みが高速化された。特に複数のHTTPベースサーバーを管理しているユーザーに効果がある。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## /security-reviewコマンド

コード変更のセキュリティ脆弱性を分析するための`/security-review`スラッシュコマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## /chronicle cost-tipsサブコマンド

パーソナライズされたトークン使用量とコスト削減ガイダンスを提供する`/chronicle cost-tips`サブコマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## preMcpToolCallフック

`preMcpToolCall`フックが追加され、プロバイダーが送信されるMCPリクエストのメタデータを制御できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## メモリ機能の改善

`/memory on|off|show`コマンドによる永続的ストレージのメモリ機能が改善された。`/memory show`でCopilot Memoryの管理に関するドキュメントリンクが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## レスポンシブな入力エリア

入力エリアが3行で固定される代わりにターミナルの高さに応じて自然に拡大するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## シークレットスキャンの拡張

シークレットスキャンがコミットメッセージとPR説明にまで拡張され、公開前のリダクションが行われるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## ターミナルプログレスインジケーター

OSC 9;4によるターミナルプログレスインジケーターが追加され、新しい`terminalProgress`設定で制御できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)

## バグ修正

設定ファイルの更新時に無関係な設定キーが蓄積される問題が修正された。リストアイテム内のGFMテーブルとブロッククォートがフローティングボーダーなしで正しくレンダリングされるようになった。ローディングインジケーターの色がアクティブモードに一致するようになった。使用量ベース課金ユーザーのセッション名設定が正常に動作するようになった。サブコマンド補完のEnterキー選択が正しく動作するようになった。Ctrl+Gエディタのキーストローク横取り問題が修正された。シェルツールのモデルが`description`パラメータを省略した場合でもツール呼び出しが成功するようになった。OAuthベースMCPサーバーの接続が認証セッション間で維持されるようになった。実験的モードインジケーターが一時的通知からアプリヘッダーの常時表示に変更された。リモートセッション起動失敗が明示的にリクエストされた場合のみ表示されるようになった。入力トークン使用量のフォーマットが改善され、キャッシュトークンが含まれるようになった。ログインプロンプトがプレーンテキスト設定ファイルのフォールバックについてより明確に警告するようになった。GitHub MCP Web検索ツールがツール検索なしですぐに利用可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.51)
