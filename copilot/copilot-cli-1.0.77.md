## ブラウザベースOAuthログインフローのデフォルト化

ローカルの対話型ターミナルにおいて、`copilot login`のデフォルトとしてブラウザベースのOAuthログインフローが採用された。リモートやヘッドレスターミナルではデバイスコード認証がデフォルトのまま維持される。`--web-flow`や`--device-code`フラグで特定の認証モードを強制でき、`/login`コマンドから対話的に選択することも可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.77)

## サンドボックスの自動無効化

無条件のオートパイロット承認を行うと、バイパスが許可されている場合に現在のセッションのサンドボックスが自動的に無効化されるようになり、ワークフローが簡素化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.77)

## マネージドサンドボックスポリシーのMDM設定による強制

macOSおよびWindowsのネイティブMDM（モバイルデバイス管理）設定を通じて、マネージドサンドボックスポリシーの強制がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.77)

## Ctrl+Gによるask_user回答の編集

新しいCtrl+Gキーボードショートカットにより、`ask_user`のフリーフォーム回答をプロンプトを閉じずに編集できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.77)

## Reasoning Effortパラメータの省略対応

Reasoning Effortパラメータを省略できるようになり、サーバー側で適切なデフォルト値が自動選択されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.77)
