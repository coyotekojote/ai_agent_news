## メモリ検索の正規化マッチング

メモリ検索に正規化マッチングが追加され、検索精度が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.7)

## ウィンドウ付きマルチクエリメモリ検索

メモリ検索でウィンドウ付きマルチクエリがサポートされ、より柔軟な検索が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.7)

## Memories MCP のドットパス非表示

Memories MCP の list、read、search からドットパス（隠しファイル）が非表示になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.7)

## Windows サンドボックス準備状態 RPC の追加

Windows サンドボックスの準備状態を確認する RPC が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.7)

## /goal の目的文字列長バリデーション

TUI で `/goal` の目的文字列の長さがバリデーションされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.7)

## ゴールライフサイクルメトリクスの追加

ゴールのライフサイクルに関するメトリクスが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.7)

## 未使用の list_dir ツール削除

実験的な `list_dir` ツールが未使用のため削除された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.7)

## バグ修正

- サンドボックスの advisory system bwrap スタートアッププローブが制限された
- TUI で同サイズの大きなペーストに対する外部エディタ展開が修正された
- レガシー通知の非推奨化が取り消された
- `fork --last` の cwd フィルタリングが修正された
- TUI で大きなペーストのプレースホルダー番号付けが Ctrl+C 後に正しく動作するよう修正された
- tmux 内で `/copy` がパススルーなしで動作するよう修正された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.7)
