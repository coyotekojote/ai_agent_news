## postToolUseフックのadditionalContext改善

postToolUseフックのadditionalContextがサイレントに破棄される代わりに、モデルへのシステムメッセージとして注入されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## /chronicle searchサブコマンドの追加

新しい`/chronicle search`機能が追加され、すべてのセッションコンテンツからキーワードやトピックベースの検索が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## /userスイッチの改善

取得済みユーザーリストの再利用と、初回アクセス時のローディングスピナー表示が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## MCP OAuthトークンの永続化

静的OAuthクライアント設定のトークンリフレッシュ操作が正しく永続化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## Alpine Linuxサポートの追加

musl libcを使用するAlpine Linuxシステムでの動作がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## /exit printオプションの追加

セッションを閉じる前にターミナルに表示する新しいフラグが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## /rubber-duckコマンドの追加

独立したエージェントによる批評を提供する実験的な`/rubber-duck`コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## /session idサブコマンドの追加

現在のセッションIDの表示とクリップボードへのコピーが可能な`/session id`サブコマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## auth.redirectPort設定の追加

MCPサーバーがOAuthコールバックを固定ポートにピン止めできる`auth.redirectPort`設定が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## /memoryスラッシュコマンドの追加

永続メモリのオン/オフ切り替えやステータス確認ができる`/memory`スラッシュコマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## copilot plugin update --allの追加

`copilot plugin update --all`によるインストール済みプラグインの一括更新が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## 入力プロンプトの折りたたみ

入力プロンプトが空の場合に折りたたまれ、入力中に自然に拡張されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## ACPクライアントへのファイルdiff報告

すべてのエディットツールタイプに対してACPクライアントへのdiffが正しく報告されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## プロンプトモードでのリポジトリフック読み込み

プロンプトモード（`-p`）で、フォルダが信頼済みの場合に`.github/hooks/`からフックが読み込まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## Windowsターミナルの文字表示改善

非UTF-8ターミナルで罫線文字やブロック文字が正しく表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## MCP設定のargs省略対応

`args`フィールドのないMCPサーバー設定が受け入れられ、空リストとして扱われるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## ドキュメント添付パスの改善

ドキュメント添付にパスが含まれるようになり、Windowsの「パスとしてコピー」入力がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## MCPタイプ表示の改善

MCPサーバーのタイプが「local」ではなく「stdio」と表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## tmuxでのプログレスバー表示修正

tmuxセッション内でプログレスインジケーターが正しく表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## 実験的コマンドのラベル表示

実験的コマンドがヘルプやピッカーで「(experimental)」ラベル付きで表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## 自動アップデートの最適化

利用可能な場合により小さなプラットフォーム固有パッケージをダウンロードするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)

## GitHub参照の自動リンク

レスポンス内のIssue/PR参照（owner/repo#number形式）が自動的にリンクされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49)
