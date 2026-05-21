## agent-tuiおよびtui-testerスキルの追加

`agent-tui`および`tui-tester`スキルが追加され、TUI関連のエージェント機能が拡張された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)

## LocalSessionInvocation機能の追加

コア機能として`LocalSessionInvocation`が追加され、ローカルセッションの呼び出しが可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)

## RemoteSessionInvocation機能の追加

コア機能として`RemoteSessionInvocation`が追加され、リモートセッションの呼び出しが可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)

## content-utilsのコンパイル時網羅性チェック強化

コアのcontent-utilsにコンパイル時の網羅性チェックが強制されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)

## PowerShell Core優先設定

WindowsでレガシーのWindows PowerShell 5.1よりもPowerShell Core（pwsh.exe）が優先されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)

## 非インタラクティブモードでのMCPサーバー設定対応

非インタラクティブモードでもMCPサーバーの設定が可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)

## Sublime TextおよびEmacsクライアントエディタのサポート

Sublime TextとEmacsクライアントエディタのサポートが追加され、ドキュメントが拡充された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)

## AgentSessionの呼び出しをagent-toolに統合

AgentSessionの呼び出しがagent-toolに統合された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)

## バグ修正・改善

セッション間のスナップショットリカバリが改善された。Windows PTYストリームでのバイナリストリーム誤検知が防止されるようになった。VimのNormalモードでマッピングされていないキーが意図せずテキストを挿入する問題が修正された。A2Aサーバーのデフォルトポリシー読み込みの整合性が確保された。ファイルストレージマイグレーションの例外処理が改善された。カスタムコマンドファイルインジェクションにおけるパストラバーサル脆弱性が防止された。グローバルfetchディスパッチャーで`NO_PROXY`環境変数が尊重されるようになった。MCPツールのnullable配列型の処理が修正された。proxy-agentのESMバンドルエクスポートが保持されるようになった。子プロセスの入出力に対する決定論的エンコーディングが提案された。CLIのInk workerエントリバンドルが改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260521.g57c42a5c4)
