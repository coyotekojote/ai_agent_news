## ネストされたプランディレクトリの重複と相対パスポリシーの修正

ネストされたプランディレクトリが重複して作成される問題が修正された。プランディレクトリ参照が絶対パス（例: `/tmp/plans/`）から相対パス（例: `../plans/`）に変更された。プラン内のネストされたサブディレクトリ（例: `architecture/frontend-v2.md`）の適切な処理が追加された。複数の設定実装に `getProjectRoot()` メソッド呼び出しが追加され、`promptProvider.ts` で `makeRelative()` ユーティリティによる相対パス変換が使用されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.39.0-preview.1)
