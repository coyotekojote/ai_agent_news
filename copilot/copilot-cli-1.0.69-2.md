## `/rubber-duck`コマンドの事前認証ヘルプ表示

`/rubber-duck`コマンドが認証前のヘルプおよびセルフドキュメントに表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## CLI OAuthコールバックによるMCPサーバー認証

CLIのOAuthコールバックフローを通じてMCPサーバーに認証できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## タイムライン満杯時のプロンプト表示改善

タイムラインが満杯の際に、ヒントバーがターミナル下部にクリッピングされる問題が修正され、`/user`切り替えピッカーの表示が改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## `/diff`でのディレクトリ内未追跡ファイルの追跡修正

`/diff`のローカル編集で、ディレクトリ内の未追跡ファイルが正しく含まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## 画面外スクロール時のプロンプト折りたたみ修正

画面より高いプロンプトが上方にスクロールした際に、ピン留めヘッダーに折りたたまれてしまう問題が修正され、スクロール可能な状態が維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## Copilotログイン必須化

ACP認証が成功を返す前にCopilotログインが必須となった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## ストリーム無効時のアシスタント応答表示修正

`--stream`が無効な場合のプロンプトモードで、アシスタントの完全な応答が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## リポジトリスコープのプラグインMCPサーバー切断修正

リポジトリがプラグインを無効にした場合や、セッションが宣言リポジトリを離れた場合に、リポジトリスコープのプラグインMCPサーバーが正しく切断されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## 非インタラクティブモードでの`copilot init`ハング修正

非インタラクティブモードで`copilot init`がハングする問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## 空の`--session-id`および`--resume`値の拒否

空の`--session-id=`および`--resume=`値が無視されずに拒否されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## タイムラインツール引数の絵文字保持修正

切り詰められたタイムラインツール引数内の絵文字が正しく保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## `/terminal-setup`出力のShift+Enter表示修正

`/terminal-setup`出力でプレーンな`Shift+Enter`が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## 小数ミリ秒トークンタイミングでのセッション再開修正

小数ミリ秒のトークンタイミングを含むセッションの再開が正しく動作するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)

## `[DIR]`で始まるファイルの@メンション補完修正

`[DIR]`で始まるファイルに対する@メンション補完が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69-2)
