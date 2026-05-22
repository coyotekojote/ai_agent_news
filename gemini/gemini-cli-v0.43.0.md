## Editツールステアリング

モデルがコードの外科的な修正に対してEditツールを使用するよう誘導されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)

## セッションのエクスポート・インポート機能

セッションをファイルにエクスポートし、フラグ指定でインポートできるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)

## Autoモードの統合

複数のAutoモードが単一のAutoモードに統合された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)

## シェルコマンド安全性評価フレームワーク

シェルコマンドの安全性を評価する新しいフレームワークが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)

## サブエージェントプロトコルの導入

`LocalSubagentProtocol`および`RemoteSubagentProtocol`の実装が導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)

## マシンホスト名の表示

CLIインターフェースにマシンのホスト名が表示されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)

## 適応型トークンカリキュレータ

コンテンツサイズの計算精度を向上させる適応型トークンカリキュレータが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)

## ツールIDプレフィックス

ツール呼び出しIDにツール名がプレフィックスとして付与されるようになり、IDEレンダリングがサポートされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)

## バグ修正・改善

コンテキストマネージャのチャット破損が修正された。YOLO/AUTO_EDITモードでサンドボックスなしのリダイレクションが修正された。非インタラクティブモードでの`AgentExecutionStopped`のJSON出力が修正された。無効なカスタムプランディレクトリがグレースフルに処理されるようになった。ツール完了待機の競合状態が解消された。サンドボックスコンテナ名がランダム化されるようになった。ヘッドレスLinuxでのOAuth時のサイレントハングが防止された。Flashクォータ枯渇後のモデル選択が適切に反映されるようになった。並列ツール呼び出しストリーミングのIDコリジョンが解消された。ドロップされたツールレスポンスが明示的なエラーをスローするようになった。Git環境でのシステムPATH保持によるENOENTエラーが修正された。VS Codeでの現在のファイル実行の実装が修正された。macOSバイナリの実行ビットが保持されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0)
