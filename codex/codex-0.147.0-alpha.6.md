## サーフェスごとのMCPツール公開制御の追加

MCPサーバーがダイレクト、遅延、コードモードの各ツールサーフェスに対して個別にオプトアウトできるようになった。

[参考リンク](https://github.com/openai/codex/pull/36781)

## Guardianセッションの再利用と中断テストの追加

ツールレビューにおけるセッション再利用と中断処理のテストが追加された。

[参考リンク](https://github.com/openai/codex/pull/36782)

## モデル命令のModelMessagesへの統合

インメモリの命令ソースを廃止し、統一テンプレートアプローチに移行した。

[参考リンク](https://github.com/openai/codex/pull/36787)

## プラグイン使用説明のモデル能力によるゲート制御

モデルメタデータフラグを追加し、プラグインガイダンスの出力を制御できるようになった。

[参考リンク](https://github.com/openai/codex/pull/36792)

## タイムアウトしたGitプロセスツリーの終了処理

タイムアウト時のクリーンアップ処理が改善され、UnixおよびWindows上でプロセスツリー全体を確実に終了させるようになった。

[参考リンク](https://github.com/openai/codex/pull/36793)

## Agent Plugins MCP設定パースの追加

Agent Plugins v1設定をCodex MCPサーバー形式に変換する機能が追加された。

[参考リンク](https://github.com/openai/codex/pull/36796)

## rusty_v8チェックサムマニフェストの改行正規化

プラットフォーム間でLF改行に統一された。

[参考リンク](https://github.com/openai/codex/pull/36797)

## ネットワークポリシーイベントキャプチャの安定化

同時テストにおいてトレーシングサブスクライバーがない場合にネットワークポリシーのコールサイトが無効としてキャッシュされる問題が修正された。

[参考リンク](https://github.com/openai/codex/pull/36779)
