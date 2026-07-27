## Windows実行のyieldフロアを10秒に引き上げ

Windows環境での非同期実行における最小yield時間が10秒に引き上げられた。

[参考リンク](https://github.com/openai/codex/pull/35670)

## Windowsの非TTYプロセスを割り込み時に終了

Windows環境において、非TTYプロセスが割り込み（interrupt）発生時に適切に終了されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35655)

## キャッシュ済みMCPツールをサーバー起動前に公開

MCPサーバーの起動を待たずに、キャッシュされたMCPツールが事前に公開されるようになった。ツールの利用開始が高速化された。

[参考リンク](https://github.com/openai/codex/pull/35590)

## マルチエージェント設定の設定表現間での保持

マルチエージェント設定が異なる設定表現間で正しく保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35656)

## リモート実行のネットワークポリシーコールバック有効化

リモート実行時のネットワークポリシーコールバックが有効化された。

[参考リンク](https://github.com/openai/codex/pull/35652)

## TUI入力をターミナルフォーカス復帰時に保持

ターミナルのフォーカスが復帰した際に、TUIの入力状態が保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35649)

## ターミナルターンエラーのリプレイ履歴への保持

リプレイされる履歴にターミナルターンエラーが正しく保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35524)

## v2 wait_agentスキーマでより長い待機を推奨

v2のwait_agentスキーマにおいて、より長い待機時間が推奨されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35594)

## ワールドステートにモデルとパーソナリティを追跡

ワールドステートにモデルとパーソナリティの情報が追跡されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35530)

## MCPサーバー再帰制限の引き上げ

MCPサーバーの再帰制限が引き上げられた。

[参考リンク](https://github.com/openai/codex/pull/35414)
