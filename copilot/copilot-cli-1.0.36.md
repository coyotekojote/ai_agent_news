## サブコマンドピッカーの選択インジケーター

サブコマンドピッカーでハイライトされた項目の横に選択インジケーター（>）が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## 複数ライセンス検出時のエラーメッセージ改善

複数の Copilot ライセンスが検出された場合に、直接リンク付きのより明確なエラーメッセージが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## `preToolUse.matcher` の修正

`preToolUse.matcher` が無視される問題が修正された。matcher 付きフックは正規表現に完全一致するツール名に対してのみ実行されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## `/keep-alive` コマンド

実験モードなしで `/keep-alive` が利用可能になり、Copilot CLI のアクティブ中にシステムスリープを防止できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## `/remote` コマンド

`/remote` コマンドで現在のステータスを表示し、`/remote on` および `/remote off` でリモートコントロールを切り替えられるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## 無効なスキルの非表示

無効化されたスキルがスラッシュコマンド一覧に表示されなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## 「changes」ステータスライントグル

セッション中の追加/削除行数を表示する「changes」ステータスライントグルが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## `.gitignored` ディレクトリのインストラクションファイル修正

`.gitignored` ディレクトリ内のカスタムインストラクションファイルが正しくロードされるよう修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## ダブル Esc によるキャンセル

実行中の作業をキャンセルするには Esc を2回押す必要があるようになり、意図しない中断が防止された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## デバッグログ・フィードバックバンドルの上書き防止

デバッグログやフィードバックバンドルの保存時に既存のアーカイブファイルが上書きされなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## `~/.claude/` カスタムリソースの非ロード化

`~/.claude/` からのカスタムエージェント、スキル、コマンドが Copilot CLI にロードされなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)

## Claude Opus 4.6 のデフォルト推論エフォート変更

Claude Opus 4.6 がデフォルトで中程度の推論エフォートを使用するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.36)
