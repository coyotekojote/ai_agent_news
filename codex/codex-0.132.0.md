## Python SDKのファーストクラス認証サポート

Python SDKにファーストクラスの認証機能が追加された。APIキーログイン、ChatGPTブラウザおよびデバイスコードフロー、アカウント情報の確認、ログアウトAPIが含まれる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)

## Turn APIの簡素化

テキストワークフロー向けにTurn APIが簡素化された。プレーンな文字列入力が受け付けられるようになり、ハンドルベースの実行で収集アイテム・タイミング・使用量メトリクスを含む拡張された`TurnResult`が返されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)

## codex exec resumeの--output-schemaサポート

`codex exec resume`コマンドで`--output-schema`パラメータがサポートされ、セッションコンテキストを維持しながら構造化されたJSON出力を強制できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)

## TUI起動の高速化

ターミナル機能の検出がバッチ処理されるようになり、シリアルチェックの代わりにまとめて実行されることでTUIの起動が高速化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)

## リモートエグゼキュータの標準認証

リモートエグゼキュータの登録で標準のCodex認証が使用されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)

## 画像忠実度の保持

app-serverのターンでユーザー入力およびツール出力を通じてオリジナル解像度の画像が保持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)

## バグ修正

ゴールの継続が使用量制限やブロッカーに達した際に過度にループする代わりに停止するようになった。セッションピッカーが改善され、リネームされたスレッドが`name (thread-id)`形式で表示され、ペーストされたテキストもサポートされるようになった。マルチセッションTUIの信頼性が向上し、リプレイ中のMCPコール状態が適切に処理されるようになった。リモートセッションのWebSocket接続が維持されるようになり、diffパスが正しく表示されるようになった。Windowsインストールがより安定し、npm検出と静的CRTリンキングが修正された。シャットダウンフィードバックやティア永続化などのTUIポリッシュが改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)

## ドキュメント

Python SDKのドキュメントが更新され、セットアップガイダンス、認証フローの例、簡素化されたテキストワークフローが改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)

## メモリサマリーのバージョン管理

メモリサマリーにバージョン管理が導入され、フォーマット変更時に自動的に再構築されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.132.0)
