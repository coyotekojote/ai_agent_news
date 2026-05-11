## セッションのエクスポート・インポート機能

セッションをファイルにエクスポートし、フラグ経由でインポートする機能が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## マシンホスト名のCLI表示

CLIインターフェースにマシンのホスト名が表示されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## サブエージェントプロトコルの追加

`LocalSubagentProtocol` と `RemoteSubagentProtocol` が `AgentProtocol` の背後に追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## スナップショッターの改善

コンテキスト処理のためのスナップショッター機能が改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## IDE向けツール呼び出しIDプレフィックス

ツール呼び出しIDにツール名がプレフィックスとして付与されるようになり、ACP準拠IDEでのツールレンダリングがサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## Git環境でのシステムPATH保持

Git環境でシステムPATHが保持されるようになり、ENOENTエラーが修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## ルーティングモデル引数の不一致修正

`ApprovalModeStrategy` の `resolveClassifierModel` の引数不一致が修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## 並列ツール呼び出しストリーミングIDの衝突修正

並列ツール呼び出しのストリーミング時にIDが衝突する問題が修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## 関数レスポンスターンエラーの修正

「function response turn must come immediately after function call」エラーが解決された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## ドロップされたツールレスポンスの明示的エラー

ドロップされたツールレスポンスに対して明示的なエラーがスローされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## memoryV2有効時の `/memory add` 非表示

memoryV2が有効な場合に `/memory add` サブコマンドが非表示になるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## ホームディレクトリ起動時の誤ったコマンド競合防止

ホームディレクトリからの起動時に誤ったコマンド競合が発生する問題が修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)

## モデルルーティング決定のキャッシュ

`LocalAgentExecutor` でモデルルーティングの決定がキャッシュされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260511.g1a894c18e)
