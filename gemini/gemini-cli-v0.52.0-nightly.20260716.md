## バージョンバンプ（0.52.0-nightly.20260715）

バージョンが `0.52.0-nightly.20260715.gfa975395b` にバンプされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28402)

## キャンセルされたツールレスポンスのグループ化と連続ロールの結合による400エラー防止

ツール呼び出しを拒否・キャンセルした後にフォローアップメッセージを送信すると「400 Bad Request」エラーが発生する問題が修正された。キャンセルされたツールレスポンスを1つのユーザーターンに集約し、連続する同一ロールのターンをマージする `coalesceConsecutiveRoles` ヘルパー関数が導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28407)
