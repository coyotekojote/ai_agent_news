## code-mode: セッションシャットダウンの権威化

各セッションとセルに階層的なキャンセルトークンが付与され、シャットダウンがレジストリをポーリングすることなく、認可されたアクターの完了を待機するようになった。

[参考リンク](https://github.com/openai/codex/pull/29287)

## プランモードプロンプトの更新

プランモードが関連するフォローアップ時にユーザーに実装計画をレンダリングするように変更され、実装作業のためにプランモードから抜けることが可能になった。

[参考リンク](https://github.com/openai/codex/pull/29301)

## code-mode: ドロップされたオブザベーション出力の保持

オブザベーションレシーバーが配信前に消失した場合に、yield された出力が復元されるようになり、配信失敗時に保留中のフロンティア出力が保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29288)

## code-mode: 完了時の初期 yield の保持

セルがオブザベーション前に完了した場合に、最初の yield_control() 境界が保持されるようになり、一貫したレスポンス境界が確保された。

[参考リンク](https://github.com/openai/codex/pull/29289)

## 自動コンパクション無効化フラグの追加

デフォルトで有効な `auto_compaction` フィーチャーフラグが内部エスケープハッチとして追加され、無効時に自動コンパクションをスキップできるようになった。

[参考リンク](https://github.com/openai/codex/pull/28260)

## セーフティバッファリングイベントのクライアント伝達

Responses API からの safety_buffering メタデータがデコードされ、型付きコアイベントとして app-server クライアントに転送されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29371)

## セッション ID のスレッドレジューム間の永続化

ルートセッション ID がすべてのロールアウトの SessionMeta に保存されるようになり、コールドレジューム後のエージェントツリーの一貫性が維持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29327)

## マルチエージェントモード制御の簡素化

委任ポリシーが none、explicitRequestOnly、proactive の3モードを持つ単一の multiAgentMode コントロールに統合された。

[参考リンク](https://github.com/openai/codex/pull/29324)

## リモート実行サーバーでのサンドボックスインテント適用

エグゼキューターがネイティブファイルシステムパスを使用してサンドボックスインテントを解釈・適用できるようになった。

[参考リンク](https://github.com/openai/codex/pull/29113)

## ワークスペースメッセージ API の追加

アクティブなワークスペースメッセージを取得するための account/workspaceMessages/read メソッドのバックエンドクライアント型が実装された。

[参考リンク](https://github.com/openai/codex/pull/29001)

## WebSocket イベントの冗長ログ削減

成功した WebSocket イベントの反復的なログ出力が削除され、SQLite の負荷が軽減された。

[参考リンク](https://github.com/openai/codex/pull/29432)
