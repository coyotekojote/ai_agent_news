## 編集ツールのステアリング改善

モデルがコードの外科的な修正にeditツールを使用するよう誘導されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.0)

## セッションのエクスポート/インポート機能

セッションをファイルにエクスポートし、フラグ経由でインポートする機能が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.0)

## マシンホスト名の表示

CLIインターフェースにマシンのホスト名が表示されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.0)

## サブエージェントプロトコルの導入

AgentProtocolの背後にLocalSubagentProtocolとRemoteSubagentProtocolが導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.0)

## ツールIDプレフィックス付与

ツールコールIDにツール名がプレフィックスとして付与されるようになり、ACP準拠のIDEでのレンダリングがサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.0)

## 適応型トークン計算

コンテンツサイズをより正確に計算するための適応型トークン計算システムが導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.0)

## シェルコマンド安全性評価

シェルコマンドの安全性評価機能が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.0)

## バグ修正

コンテキストマネージャーのチャット破損バグが修正された。ツール完了待機のレースコンディションが解消された。ヘッドレスLinuxでのOAuth認証時のサイレントハングが防止された。並列ツールコールのストリーミングID衝突が解消された。「function response turn must come immediately after function call」エラーが修正された。LocalAgentExecutorでのモデルルーティング決定キャッシュが修正された。不正なprojects.jsonの処理が改善された。サンドボックスコンテナ名がランダム化され分離が向上した。macOSバイナリの実行ビットが保持されるようになった。信頼されていないフォルダでのMCPリストUXが改善された。レガシーセッションのレジューム機能が復元された。音声文字起こしの表示タイミングが修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.0)
