## `--plugin`、`--mcp`、`--skill`フラグの追加

プラグインの変更操作用に`--plugin`、`--mcp`、`--skill`フラグが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72-1)

## スキル削除サポートの追加

`copilot plugins remove --skill`でスキルの削除がサポートされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72-1)

## コンパクト編集行展開時のフルファイルパス表示

コンパクト編集行を展開した際にフルファイルパスが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72-1)

## プラン承認メニューのモデル間一貫性向上

プラン承認メニューがモデル間で決定論的になるよう改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72-1)

## `/add-dir`ディレクトリのターン間可視性維持

`/add-dir`ディレクトリがターンをまたいでエージェントコンテキスト内で可視状態を維持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72-1)

## 分割ペインチャットビューでのask-user・elicitation入力の折り返し修正

分割ペインチャットビューでask-userとelicitation入力が正しく折り返されるように修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72-1)

## ツール権限プロンプトでのCtrl+K・大文字J/Kの動作修正

Ctrl+K、大文字のJ/Kがツール権限プロンプトや類似メニューで選択を移動しなくなった。ナビゲーションは修飾なしのj/k、矢印キー、Ctrl+P/Ctrl+Nを使用する。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72-1)

## `/terminal-setup`のJSON構文エラーを含むkeybindings.json修正拒否

`/terminal-setup`がJSON構文エラーを含むVS Codeの`keybindings.json`を書き換える代わりに変更を拒否するようになり、ドキュメントの無効JSON処理と一致するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.72-1)
