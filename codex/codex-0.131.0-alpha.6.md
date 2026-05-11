## レスポンシブMarkdownテーブルレンダリング

TUIレスポンスでテーブルがレスポンシブにレンダリングされるようになった。十分なスペースがある場合はUnicodeの罫線でボーダーが描画され、狭いペインでは行ごとの縦型レイアウトにフォールバックする。ターミナルリサイズ時の再レンダリングも正しく動作する。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.6)

## 型付きエクステンションAPI

機能が独自のコントリビューションをインストールできる、小規模な型付きエクステンションフレームワークが導入された。エクステンションレジストリがランタイムシステムを通じて接続され、スレッド・セッション起動時にホスト所有のコントリビュータストアにアクセスできるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.6)

## Gitアトリビューションのエクステンション化

Gitコミットアトリビューション機能がコアから専用エクステンションに移行され、プロンプトポリシー動作がセッションオーケストレーション層から分離された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.6)

## tmuxでのShift+Enter修正

tmuxセッションでShift+Enterが正しく改行を挿入するようになった。CSI-u拡張キーフォーマットを検出し、`modifyOtherKeys` モード2をリクエストすることで修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.6)

## Windows MCPクリーンアップ改善

Windows上のMCPプロセス終了時に `taskkill` の不要なコンソール出力が抑制され、画面の破損が防止された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.6)

## Issue Digestの重複排除

Issue Digestが生のインタラクション数ではなくユニークなGitHubユーザー数でカウントするようになり、単一ユーザーによる複数のコメントやリアクションでIssueの重要度が不当に上がることが防止された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.6)

## Gitプラグインメタデータキャッシュ

Git由来のマーケットプレイスプラグインのキャッシュ済みメタデータを `plugin/list` インターフェースから読み取れるようになり、不要なクローンが排除された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.6)
