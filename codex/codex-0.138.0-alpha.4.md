## モデル定義の推論エフォート対応

モデル定義の非空の推論エフォート値がcore、app-server、TUIレイヤー全体でサポートされるようになった。モデルカタログの順序が推論選択肢に保持され、ショートカットも調整された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.4)

## AGENTS.mdの環境ファイルシステム経由ルーティング

AGENTS.mdの読み込みが選択された環境のファイルシステムを経由するようになり、リモートワークスペースでのワークスペース固有の指示読み込みが対応された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.4)

## ThinLTOによるビルド高速化

リリースバイナリがFat LTOからThinLTOに切り替えられ、ビルド時間が40%削減された（バイナリサイズは7.63%増加）。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.4)

## バグ修正・クリーンアップ

Windowsサンドボックスビルドスクリプトのclippy警告が修正された。

不要な`response.processed` WebSocketリクエストが削除された。

廃止された実験機能キーがクリーンアップされ、無効なエントリに対してエンドポイントが寛容になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.4)
