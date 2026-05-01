## アドホックメモリ拡張機能の追加

アドホックメモリ拡張の指示シードが追加され、メモリの記憶プロンプトの改善とメモリ編集機能が実装された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.2)

## Vim コンポーザーモードの追加

TUI に Vim コンポーザーモードが追加され、Vim キーバインドでの入力が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.2)

## TUI ステータスラインのテーマカラー対応

TUI のステータスラインがアクティブテーマの配色に基づいて表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.2)

## ゴール期間の複数日表示対応

TUI で複数日にわたるゴールの期間が適切にフォーマットされて表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.2)

## リモートプラグインの機能強化

- リモートプラグインのスキル読み取り API が追加された
- 認証変更時にリモートプラグインキャッシュがリフレッシュされるようになった
- 共有プラグインのローカルパス追跡が実装された
- 管理者によって無効化されたリモートプラグインのステータスが表示されるようになった
- リモートプラグインインストールのアナリティクスが送信されるようになった

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.2)

## スレッドストアのプロセススコープ化

スレッドストアがプロセススコープになり、スレッドアナリティクス状態が集中管理されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.2)

## リモートコントロールのプロトコル v3 対応

リモートコントロールがプロトコル v3 セグメンテーションに切り替わった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.2)

## バグ修正と改善

- heredoc パース時のファイルリダイレクトの問題が修正された
- Windows で PowerShell の `-Command` ラッパーがアンラップされるようになった
- `codex_hooks` フィーチャーが `hooks` としてエイリアス化された
- `thread/turns/list` と `exclude_turns` が実験的としてマークされた
- 未使用のイベントメッセージが削除された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.2)
