## リアルタイムボイスモード

クラウドとローカルバックエンドの両方に対応したリアルタイムボイスモードが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260427.g42587de73)

## 実験的 Gemma 4 モデルのサポート

実験的な Gemma 4 モデルバリアントのサポートが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260427.g42587de73)

## 自動メモリスクラッチパッドの永続化

スキル抽出用のメモリシステムにおいて、自動メモリスクラッチパッドが永続的に保存されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260427.g42587de73)

## 起動時間の改善

experiments と quota の読み込みが非同期で行われるようになり、起動時間が改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260427.g42587de73)

## セキュリティ強化

- `.env` ファイルのロードがセキュア化され、ヘッドレスモードでワークスペース信頼が強制されるようになった
- YOLO モードでシェルパースが制限ルールに失敗した場合にフェイルクローズするようになった
- シェルコマンドの検証とコアツール許可リストが追加された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260427.g42587de73)

## CLI の改善

- 部分入力が空の場合のみ `list` サジェスションを表示するよう修正された
- コマンドの出力リダイレクトが対応された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260427.g42587de73)

## バグ修正

- ループ検出時の未処理 AbortError による致命的クラッシュが修正された
- ユーザーメッセージコンポーネントの背景色チェックが修正された
- Windows でのバックスペースハンドリングのリグレッションが修正された（リバート）

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260427.g42587de73)

## ドキュメント・インフラ

- README に Gemini CLI コースリンクが追加された
- FatalUntrustedWorkspaceError にドキュメントリンクが含まれるようになった
- gemini-cli-bot メトリクスとワークフローが追加された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260427.g42587de73)
