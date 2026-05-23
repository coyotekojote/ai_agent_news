## Typed Imagesクライアントの強化

`ImagesClient`にJSON画像生成・編集リクエストの型付きリクエスト/レスポンス構造とbase64画像出力のサポートが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.3)

## コンパクション分析トラッキングの分離

リモートコンパクションv2とローカルプロンプトベースのコンパクションを区別するため、分析トラッキングに`responses_compaction_v2`値が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.3)

## SessionTaskの入力処理改善

`SessionTask::run`が`Vec<TurnInput>`を受け取るように変更され、初回入力とフォローアップ入力の差異が解消された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.3)

## 使用量制限エラーヘッダーの解析

`X-Codex-Rate-Limit-Reached-Type`ヘッダーの解析が追加され、クレジットおよび利用上限シナリオに対するワークスペース固有のエラーメッセージが表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.3)

## その他の改善

DotSlashマニフェスト処理が再利用可能なヘルパーに抽出された。プロンプト画像の再エンコーディングパスのベンチマークとスモークテストが追加された。MCPツールスキーマのJSON Schemaポリシーカバレッジテストが追加された。WebSocketセッションリセットのクライアント内部処理が整理された。macOS x64（Intel）向けzshリリースアーティファクトが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.3)
