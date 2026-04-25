## `/resume` のパフォーマンス改善

大規模セッションでの `/resume` が大幅に高速化された（40MB 以上のセッションで最大 67% 高速化）。デッドフォークエントリが多いセッションの処理も効率化された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## MCP 起動の高速化

複数の stdio MCP サーバーが設定されている場合の起動が高速化された。`resources/templates/list` は最初の `@` メンション時まで遅延されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## フルスクリーンスクロールの改善

VS Code、Cursor、Windsurf ターミナルでのフルスクリーンスクロールがよりスムーズになった。`/terminal-setup` がエディタのスクロール感度を設定するようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## 思考スピナーのインライン進捗表示

思考スピナーがインラインで進捗を表示するようになった（「still thinking」「thinking more」「almost done thinking」）。従来の別行ヒント表示を置き換えた。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## Harness インストラクションの追加

ターミナル出力、パーミッション、ツール使用に関する新しい Harness インストラクションが追加された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## Memory インストラクションの追加

よりスマートな永続メモリとクリーンアップのための Memory インストラクションが追加された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## BrowserBatch ツール

複数ステップのブラウザアクションを一括実行できる BrowserBatch ツールが追加された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## Write フローの安全性向上

Write ツールが書き込み前にファイルの読み取りを要求するようになり、安全性が向上した。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## `/config` 検索の改善

`/config` の検索がオプション値にもマッチするようになった（例：「vim」で検索するとエディタモード設定が見つかる）。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## `/doctor` の応答中オープン対応

`/doctor` が Claude の応答中でも開けるようになり、現在のターンの完了を待つ必要がなくなった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)

## バグ修正

- バックグラウンドタスクが存在する場合のアイドル再レンダーループが修正され、Linux でのメモリ増大が軽減された

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.120)
