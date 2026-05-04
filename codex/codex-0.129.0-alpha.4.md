## TUI キーマップの拡張とデバッグインスペクター

TUI のキーマップカバレッジが大幅に改善され、カスタマイズ可能なキーマップ設定が強化された。また、キーマップデバッグインスペクターが追加され、キーバインドの確認やトラブルシューティングが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.4)

## PR サマリーステータスライン

TUI のステータスラインに PR サマリー項目が追加され、現在の PR の状態を一目で確認できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.4)

## MCP サーバー命令のデファードネームスペース対応

MCP サーバーの命令（instructions）がデファードネームスペースの説明文に使用されるようになり、ツール検索時の情報がより正確になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.4)

## Memories MCP の検索・一覧機能強化

Memories MCP にマルチクエリ検索、コンテキスト行の追加、検索結果・一覧のページネーション、浅いリスト表示がサポートされた。またシンボリックリンクの走査攻撃を防止するセキュリティ強化も行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.4)

## /approvals の廃止と /autoreview の /approve へのリネーム

`/approvals` コマンドが廃止され、`/autoreview` が `/approve` にリネームされた。承認モードの `approve` に対する skip-review ハンドリングが統一された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.4)

## 推論エフォートのトレーシングスパン対応

ターンのトレーシングスパンに推論エフォート（reasoning effort）が追加され、パフォーマンス分析が改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.4)

## stdio exec-server リスナーの追加

stdio 経由の exec-server リスナーが追加され、外部プロセスとの新たな通信パスが利用可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.4)

## バグ修正

- Windows の TUI でペーストのバースト間隔が共有設定を使用するよう修正された
- TUI で修飾キー付きの Backspace/Delete キーがサポートされた
- Windows PTY のティアダウンで ConPTY の所有権が保持されるよう修正された
- Linux サンドボックスでシステムの bwrap に権限がない場合にフォールバックするよう修正された
- 一時停止中のゴールがスレッド再開時に一時停止状態を維持するよう修正された
- `/side` の親セッション復元リプレイが高速化された
- フィードバックタグに最後のモデル ID が保持されるようになった

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.4)
