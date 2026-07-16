## ターミナルセッション間のwrite_stdin並行実行

独立したターミナルセッションへの `write_stdin` が並行実行されるようになった。各セッション内ではシリアル化される。

[参考リンク](https://github.com/openai/codex/pull/33645)

## アプリメタデータ読み取りAPIの追加

最大100アプリIDのメタデータをオプションのツールサマリー付きで取得する実験的な `app/read` リクエストが追加された。

[参考リンク](https://github.com/openai/codex/pull/33651)

## スポーンロール適用後のreasoning effortバリデーション

ロールが設定を上書きする際に、最終的なreasoning effortがモデルメタデータに対して検証されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33656)

## v2サブエージェントリロード時のエージェントロール復元

再開されたセッションからリロード前にエージェントロール設定が復元されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33657)

## 設定更新時のアクティブターン環境の安定維持

各ターンでキャプチャされた環境選択が後続のステップコンテキストで保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33658)

## コードモード画像出力のdata URL制限

画像出力が `data:` スキームURLのみに制限された。

[参考リンク](https://github.com/openai/codex/pull/33659)

## 全セッションのステップワールドステート更新

各ステップ前に環境のreadiness状態とAGENTS.mdが更新されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33665)

## スタンドアロン拡張機能からのスレッドオリジネーター転送

Web検索/画像リクエストでの課金帰属のためにスレッドスコープのオリジネーターが保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33677)

## apply_patchツール説明の改訂

apply_patchツールの説明テキストが改訂された。

[参考リンク](https://github.com/openai/codex/pull/33680)

## インポートエージェントメモリのスコープと出所保持

インポートされたリソースがソースのフロントマターを保持しながら記録されるようになった。メモリサマリーに制限が設けられた。

[参考リンク](https://github.com/openai/codex/pull/33683)

## TUI承認リクエストペイロードの構造体抽出

承認リクエストがコマンド、権限、パッチ、MCPエリシテーション用の専用構造体にリファクタリングされた。

[参考リンク](https://github.com/openai/codex/pull/33684)

## 移行修復時の不要書き込み回避

修復更新を発行する前に移行履歴がチェックされ、ライタースロットの競合が防止されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33687)
