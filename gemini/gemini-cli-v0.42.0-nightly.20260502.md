## ACP エージェントモードの切断解消とモード認識改善

ACP（Agent Control Protocol）でのエージェントモード切断が解消され、モード認識が改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26332)

## サブエージェントのアクティブ承認モード認識

サブエージェントが親セッションのアクティブな承認モードを認識して適切に動作するようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/23608)

## Gemma 4 モデルのデフォルト有効化

Gemini API 経由の Gemma 4 モデルがデフォルトで有効化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26307)

## 音声モードのウェーブアニメーション追加

音声モードの UI にウェーブアニメーションが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26284)

## --prompt フラグの非推奨解除

`--prompt` フラグが非推奨から復帰し、位置引数クエリのドキュメントが修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26329)

## バグ修正

- セッション再開時にセッションスコープの状態がリセットされるようになった
- Ghostty ターミナルの raw-mode で OAuth フローが誤ってキャンセルされる問題が修正された
- `InvalidStream` イベントでの「System: Please continue.」の不要な注入が削除された
- Escape キーが入力バッファを誤ってクリアする問題が修正された
- プロンプトスニペットでの無差別な `git add .` の実行が抑制された
- バイナリでのデーモン再起動が有効化され、keytar がバンドルされた
- `.env` での `GOOGLE_CLOUD_PROJECT` の上書きが正しく尊重されるようになった
- ボックスエッジの表示問題が修正された
- 音声転写がカーソル位置に正しく挿入されるようになった
- ジェネラリストプロファイルの残存する問題が一括修正された

[参考リンク](https://github.com/google-gemini/gemini-cli/commits/main/?since=2026-05-01&until=2026-05-02)
