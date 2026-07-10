## スクラブ済み履歴ターンからの思考ストリップとリーク解消

スクラブされた履歴ターンから思考（thoughts）をストリップし、思考リークを解消する修正が行われた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27971)

## ワークスペースコンテキストからの一時的CIファイル除外

一時的なCI設定ファイルがワークスペースコンテキストから除外されるようリファクタリングされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28216)

## トリアージワーカーのコア基盤モジュール追加

caretaker-triageにトリアージワーカーのコア基盤モジュールが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28163)

## Octokit GitHubアクションハンドラーの実装

caretaker-egressにOctokitを使用したGitHubアクションハンドラーが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28303)

## JSONおよびIPYNBファイルのLLM補正バイパス

`write_file`および`replace`でJSONおよびIPYNBファイルに対するLLM補正がバイパスされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28223)

## フォールバックサマリーの曖昧でないラベル使用

フォールバックサマリーにおいて曖昧でない「previous intent」ラベルが使用されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28343)

## トリアージワーカーのメイン実行ループとエグレスアクションパブリッシャーの実装

caretaker-triageにメインワーカー実行ループとエグレスアクションパブリッシャーが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28306)
