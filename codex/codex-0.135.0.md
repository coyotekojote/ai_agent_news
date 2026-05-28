## 診断機能の強化

`codex doctor`が環境、Git、ターミナル、app-server、スレッドインベントリに関するより詳細な診断レポートを出力するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.135.0)

## /statusコマンドの拡張

`/status`コマンドがリモート接続情報とサーバーバージョンを表示するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.135.0)

## Vimモードの改善

テキストオブジェクト編集、単語・行末の動作改善、割り込みターンバインディングの設定が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.135.0)

## パーミッションプロファイル

`/permissions`コマンドが名前付きパーミッションプロファイルに対応し、カスタムプロファイルの表示が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.135.0)

## パッケージビルドの改善

パッケージ版CodexがmacOS/Linuxでバンドルされたパッチ済みzshヘルパーを検出できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.135.0)

## Python SDKの改善

Python SDKでスレッドおよびターンAPIに対応するフレンドリーな`Sandbox`プリセットが公開された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.135.0)

## バグ修正

Markdownテーブルと複数行リストのカラムサイズ表示改善、macOSおよびZellijでのTUI出力安定性向上、スラッシュコマンド補完時のドラフトテキスト保持、古いtmux/iTermセッションでのCtrl-Cハンドリング修正、アクセス不可アプリのメンション除外、非インタラクティブexecセッションの再開フローにおけるcwdオーバーライド対応が行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.135.0)

## メンテナンス

RustツールチェーンおよびSQLx/SQLite依存関係の更新、メモリランタイム状態の専用SQLiteデータベースへの移行、レスポンスリトライ処理とMCPツール命名ロジックの集約が行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.135.0)
