## `/autopilot` スラッシュコマンドの追加

インタラクティブモードとオートパイロットモードを切り替える `/autopilot` スラッシュコマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.45)

## Windows PowerShell フォールバック

WindowsでPowerShell 7+（pwsh）が利用できない場合、Windows PowerShell（powershell.exe）にフォールバックするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.45)

## OpenTelemetry の改善

OpenTelemetry出力がGenAIセマンティック規約に準拠するようになった。MCPツール呼び出しが標準的な tool_call スパンを使用し、新しい `gen_ai.client.operation.duration` メトリクスでツール実行時間を追跡できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.45)

## セッション再開の修正

拡張機能の権限プロンプトを含むセッションが「Session file is corrupted」エラーなしで再開できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.45)

## agentStop フックの修正

エージェントが task_complete で停止した場合に agentStop フックが正しく発火するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.45)

## CLI起動の高速化

OSCカラークエリのサポートが限定的なターミナルでのCLI起動が高速化され、起動時間が最大約1.5秒短縮された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.45)

## `/fork` コマンドの追加

現在のセッションを新しい独立したセッションにフォークする `/fork` コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.45)
