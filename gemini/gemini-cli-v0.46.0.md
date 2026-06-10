## PTYリサイズのクラッシュ耐性強化

PTYリサイズ処理がネイティブクラッシュに対して堅牢化された。ターミナルのリサイズ時の安定性が向上した。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.46.0)

## 無効なpreferredEditorによるスパムループ防止

`preferredEditor`が無効な値に設定されている場合にスパムループが発生する問題が修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.46.0)

## Flash GAモデルへの移行

実験フラグが有効な場合、Flash GAモデルに移行されるようになった。新しいAIモデルバリアントの採用が進められた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.46.0)

## CIワークフローの改善

PRサイズラベラーの最適化とワークフローのバッチ処理が導入された。フォークPRに書き込みアクセスを付与するため`pull_request_target`トリガーが使用されるよう修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.46.0)
