## リモートコントロールの接続保持修正

WebSocketハンドシェイクのエラーハンドリングが改善され、明示的なサーバー未検出レスポンスと一般的な404エラーが区別されるようになった。特定のエラーメッセージの場合のみエンロールメントがクリアされ、未認識のレスポンスでは保持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## プラグインサービスへのプロダクトSKU送信

プラグインサービスとの通信にCodexプロダクトSKUが含まれるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## rusty_v8の更新

V8 JavaScriptエンジンバインディングがv149.2.0に更新された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## サンドボックス承認決定の保持修正

統一実行パスでのサンドボックスセマンティクスが修正された。特にzsh-forkランタイムにおいて、承認済みサンドボックス決定が起動およびインターセプト実行パスを通じて永続化されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## resumeとforkでのプロンプト受け付け

`codex resume --last`および`codex fork --last`が初期プロンプトをセッション識別子として扱わず、正しく受け付けるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## MCP起動ステータスのスレッドスコープ化

MCPサーバーの起動通知が所属スレッドに分離され、子エージェントの失敗による親トランスクリプトの汚染が防止された。プロトコルにスレッド所有権トラッキングが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## コードモードでのスタンドアロンWeb検索

スタンドアロン検索APIからのプレーンテキスト出力の消費が追加され、コードモードで`web.run`が公開された。ネストされたJavaScript呼び出しに検索結果を返すことが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## v2エージェントレジデンシーLRU

マルチエージェントv2サブエージェント向けにLRUベースのレジデンシー管理が実装された。セッション容量が一杯になった際にロード済みエージェントをページアウトしつつ、論理的なアイデンティティを維持できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## v2同時実行カウントの改善

マルチエージェントv2の同時実行制限が、レジデントエージェント数のカウントからアクティブな非ルートターンのカウントに変更された。RunningTaskで管理されるRAIIガードが使用される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)

## close_agentからinterrupt_agentへのリネーム

v2ツールオペレーションが`close_agent`から`interrupt_agent`にリネームされ、エージェントの可用性を削除せずに現在のターン実行を中断するという動作をより正確に反映するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.7)
