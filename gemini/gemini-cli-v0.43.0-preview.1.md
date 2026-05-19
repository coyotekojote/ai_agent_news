## a2a-serverのデフォルトポリシーローディング実装

a2a-serverにデフォルトポリシーローディングが実装され、CLIとの動作の一貫性が確保された。以前はサーバーが非YOLOモードで空のポリシールールで初期化されていたが、`createPolicyEngineConfig`関数を通じてデフォルトポリシーが読み込まれるようになった。信頼されていないワークスペースが`adminPolicyPaths`や`policyPaths`などのセキュリティに関わる設定を上書きすることを防止する信頼性検証チェックも追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.43.0-preview.1)
