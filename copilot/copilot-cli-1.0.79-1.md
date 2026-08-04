## サンドボックス設定名の変更（破壊的変更）

サンドボックス設定の`allowDevToolCaches`が`allowDevToolAccess`にリネームされた。キャッシュだけでなくdev-toolの設定やレジストリも対象範囲に拡大された。古い設定を`false`に設定しているユーザーはデフォルトの有効状態に戻るため、`settings.json`およびマネージド/MDMポリシーの更新が必要。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.79-1)

## コンテキストアトリビューション計算の改善

コンテキストアトリビューション計算がAuto解決されたモデルに対して実行されるようになり、FreeおよびStudentティアのユーザーに対して正確なトークンカウントが報告されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.79-1)

## 拡張無効化時の不具合修正

拡張を無効化した際に他の拡張のelicitation、canvas機能、ツール権限プロンプトに影響を与える問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.79-1)

## プロンプト保存の永続化修正

Ctrl+Sで保存されたプロンプトが元のセッションに関連付けられた状態を維持するようになった。コンテキストを切り替えた後も保存されたプロンプトを復元できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.79-1)

## Linuxサンドボックスバイパス動作の改善

Linuxシステムで検索やシェルコマンドがサンドボックス制限に遭遇した場合、サンドボックス外でコマンドを再実行するオプションが提示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.79-1)
