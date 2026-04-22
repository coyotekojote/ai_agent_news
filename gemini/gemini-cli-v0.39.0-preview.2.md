## エージェントリフレッシュ時の重複初期化呼び出しの修正

`/agents reload` 実行時に `initialize()` が重複して呼び出され、A2AClientManager でリモートエージェントに「already loaded」エラーが発生する問題が修正された。`onAgentsRefreshed` ハンドラから不要な `initialize()` 呼び出しが削除された。テストがプライベートメソッドではなく公開 API `getAgentRegistry().reload()` を使用するよう更新され、二次的なストリーミング問題も修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.2)
