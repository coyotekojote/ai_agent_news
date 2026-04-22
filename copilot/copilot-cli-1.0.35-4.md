## セッションの名前付きレジュームサポート

`--name` でセッションに名前を付け、`--resume=<name>` で名前を指定してレジュームできるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35-4)

## LSP サーバーのタイムアウト設定

`lsp.json` の LSP サーバーエントリで、スポーン、初期化、ウォームアップのタイムアウトが個別に設定可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35-4)

## コンテキストウィンドウインジケーターの非表示化

ステータスラインのコンテキストウィンドウインジケーターがデフォルトで非表示になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35-4)

## MCP OAuth の改善

MCP OAuth 機能が共有ランタイムフローに統合された。MCP サーバー削除時に OAuth 状態がクリアされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35-4)

## バグ修正

- Windows で「Configure Copilot」エージェントがシェルアクセスを持つようになった
- Linux でクリップボードユーティリティ（`wl-clipboard` または `xclip`）が見つからない場合にインストール手順を含むエラーメッセージが表示されるようになった

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35-4)
