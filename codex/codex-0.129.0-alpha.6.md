## セッションピッカーのリデザイン

TUI のセッションピッカーが再設計され、セッション一覧の操作性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.6)

## /diff のワークスペースコマンド経由ルーティング

`/diff` がワークスペースコマンドを経由してルーティングされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.6)

## モデルサービスティアメタデータの追加

モデルにサービスティアメタデータが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.6)

## 大きなフック出力のコンテキスト外退避

大きなフック出力がコンテキストからスピルされ、コンテキストウィンドウの消費が抑制されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.6)

## PreToolUse の additionalContext サポート

`PreToolUse` フックで `additionalContext` がサポートされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.6)

## スキル呼び出しアナリティクスの改善

スキル呼び出しアナリティクスに `turn_id` とプラグイン ID が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.6)

## バグ修正

- Linux サンドボックスの合成マウントレジストリがユーザーごとに分離されるよう修正された
- Linux サンドボックスで bwrap ビルド失敗時のパニックが回避された
- ネットワークプロキシで DNS タイムアウトブロッキングがカバーされた

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.6)
