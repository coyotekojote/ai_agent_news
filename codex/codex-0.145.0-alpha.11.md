## exec-server JSON-RPCデコード複雑度の制限

メッセージが256K値に制限され、重複キーが拒否され、ディレクトリ/プロセス出力が50,000エントリに制限された。

[参考リンク](https://github.com/openai/codex/pull/33013)

## TypeScriptエンベロープへのrawレスポンスCompletions追加

TypeScriptエンベロープにrawレスポンスCompletionsが含まれるようになった。

[参考リンク](https://github.com/openai/codex/pull/33026)

## list_agents出力からのタスクメッセージ削除

`list_agents`の出力からタスクメッセージが削除された。

[参考リンク](https://github.com/openai/codex/pull/33030)

## exec-server RPCメッセージのJSON数値精度保持

exec-serverのRPCメッセージでJSON数値の精度が保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33031)

## プロンプトキャッシュキーへのセッションID使用

プロンプトキャッシュキーにセッションIDが使用されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33035)

## APIキー認証でのプラグイン分析送信

プラグイン分析がAPIキー認証で送信されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33040)

## エージェント拡張ランナーの追加

解決済みエージェントプロンプトをフォークされたスレッドで起動するAgentRunnerが導入された。

[参考リンク](https://github.com/openai/codex/pull/33076)
