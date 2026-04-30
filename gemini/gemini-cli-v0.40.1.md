## テレメトリの logPrompts フラグ対応

`logPrompts` 設定フラグが無効の場合に、ユーザープロンプト、ポリシー、コンテンツ、判定理由などの機密フィールドが OpenTelemetry および Clearcut のログから除外されるようになった。以前はプライバシー設定に関係なく機密情報がログに記録されていた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.1)
