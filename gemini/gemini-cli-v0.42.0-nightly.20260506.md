## a2a-server のツール承認レースコンディション修正

複数のツール確認が同時に処理される際にシステムがハングする同期の問題が修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260506.g80d269054)

## 圧縮中のメッセージキューイング

圧縮処理中にメッセージをキューイングできるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260506.g80d269054)

## 編集ツールへのモデル誘導

外科的な編集に対してモデルが edit ツールを使用するよう誘導されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260506.g80d269054)

## Auto Memory ドキュメントの明確化

Auto Memory がメモリの更新とスキルを提案する旨がドキュメントで明確化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260506.g80d269054)

## YOLO/AUTO_EDIT モードでのリダイレクション許可

YOLO および AUTO_EDIT モードでシェルコマンドのリダイレクション（例: `npm test 2>&1 | tail -80`）がサンドボックスの有無に関係なく許可されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260506.g80d269054)

## macOS バイナリのリリース添付

CI でビルドされた未署名の macOS バイナリがリリースに添付されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260506.g80d269054)

## バグ修正

- 設定ダイアログの枠線が `maxHeight` を使用してクリッピングされないよう修正された
- `ERR_STREAM_PREMATURE_CLOSE` エラー時にリトライされるようになった
- ジェネラリストプロファイルの軽微な修正が行われた
- `GOOGLE_CLOUD_PROJECT` で数値プロジェクト ID が拒否されるようになった
- エラーユーティリティの unsafe な型アサーション抑制が削除された
- コンテキストマネージャーのチャット破損バグが修正された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260506.g80d269054)
