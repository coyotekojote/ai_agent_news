## ChatGPTのAgent Identity認証オプトイン

ChatGPTログインのCodexセッション向けに、バックエンド経由でAgent Identityランタイム認証がデフォルト無効で追加された。

[参考リンク](https://github.com/openai/codex/pull/19049)

## 合成リンクのアプリアクセシビリティ除外

合成MCPツールをアプリのアクセシビリティの証拠として扱わないようになった。エージェントワークフロー向けには引き続き保持される。

[参考リンク](https://github.com/openai/codex/pull/28770)

## リモートプラグインダウンロードステータスエラーの保持

リモートプラグインバンドルのダウンロード失敗時に、元のHTTPステータスコードが保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28863)

## 外部環境からのAGENTS.md読み込み

異なるOSのリモートexec-serverからAGENTS.mdを読み込めるようになった。

[参考リンク](https://github.com/openai/codex/pull/28958)

## マーケットプレイスプラグインマニフェストのフォールバック

発見可能なマニフェストがないマーケットプレイスプラグインが、marketplace.jsonエントリをフォールバックマニフェストとして使用できるようになった。

[参考リンク](https://github.com/openai/codex/pull/28789)

## 子AGENTS.mdプロンプト実験の削除

無効化されていた「child_agents_md」実験的機能と関連設定が削除された。

[参考リンク](https://github.com/openai/codex/pull/28993)

## AGENTS.mdパスのURIログ出力

内部ログでAGENTS.mdパスがURI形式で出力されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28989)

## リモートexecのシェル制限

リモートコマンド実行が環境のデフォルトシェルに制限され、ホスト側のシェル解決を回避するようになった。

[参考リンク](https://github.com/openai/codex/pull/28983)

## プラグインスキルの再利用パース

セッション起動時にプラグインスキルのパース結果がキャッシュ・再利用され、重複パースが排除された。

[参考リンク](https://github.com/openai/codex/pull/28844)
