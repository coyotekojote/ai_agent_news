## Windows バックスペースハンドリングのリグレッション修正

Windows でのバックスペースキーの処理に関するリグレッションが修正された。Windows Terminal 向けの環境固有チェックが削除され、`\b` と `\x7f` の両方が全プラットフォームで標準的なバックスペース入力として統一的に処理されるよう簡素化された。v0.40.0-preview.3 からのチェリーピック修正。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.4)
