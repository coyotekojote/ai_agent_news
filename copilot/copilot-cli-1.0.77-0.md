## ブラウザベースOAuthログインフローの追加

ローカルの対話型ターミナルにおいて、`copilot login`のデフォルトとしてブラウザベースのOAuthログインフローが追加された。リモートやヘッドレスターミナルではデバイスコード認証がデフォルトのまま維持される。`--web-flow`や`--device-code`フラグで特定の認証モードを強制でき、`/login`コマンドから対話的に選択することも可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.77-0)

## マネージドサンドボックスポリシーのMDM設定による強制

macOSおよびWindowsのネイティブMDM（モバイルデバイス管理）設定を通じて、マネージドサンドボックスポリシーの強制がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.77-0)

## Reasoning Effortパラメータの省略対応

Reasoning Effortパラメータを省略できるようになり、サーバー側で適切なデフォルト値が自動選択されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.77-0)
