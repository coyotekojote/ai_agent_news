## 設定ロックファイルのエクスポートとリプレイ機能

セッションの解決済み設定状態をエクスポートできるようになった。`debug.config_lockfile.export_dir` でロックファイルを出力し、`debug.config_lockfile.load_path` で保存済み設定をリプレイできる。ロックファイルにはモデル選択、フィーチャー状態、サービスティアなどの解決済み値が含まれ、プロファイル/デバッグ/環境固有の入力はストリップされる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.3)

## Apply-Patch のファイル変更をターンアイテムとして統合

apply-patch のファイル変更がレガシーパッチイベントではなくコアターンアイテム（`TurnItem::FileChange`）として構造化された。`ItemStarted`/`ItemCompleted` 通知が送信され、API クライアント間で一貫した消費パターンが実現された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.3)

## アクセシビリティ向けアニメーション無効化対応

`tui.animations = false` 設定時にスクリーンリーダー互換性が改善された。ライブステータス行のスピナーが省略され、実行中フックヘッダーがスピナープレフィックスなしで表示されるようになった。スピナー使用が `motion.rs` モジュールに集中管理された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.3)

## /goal コマンドの継続ロジック簡素化

`/goal` コマンドの処理から早期終了ヒューリスティクスが削除され、進行可能な場合に早期停止しなくなった。ブロック時にモデルに待機を指示する継続プロンプトや、ツール未使用ターン後の継続抑制が削除された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.3)

## TUI での IDE コンテキストサポート

`/ide [on|off|status]` コマンドが追加され、TUI から IDE 拡張機能との IPC 通信を介してライブ IDE コンテキスト（開いているファイル、選択範囲）にアクセスできるようになった。ステータスラインに IDE コンテキストのアクティブ状態が表示される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.3)

## App-Server トランスポート層のリファクタリング

トランスポート実装が `codex-app-server-transport` クレートとして分離された。stdio、Unix ソケット、WebSocket、リモートコントロールの各トランスポートが新クレートに移動し、アーキテクチャ境界が明確化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.3)

## セキュリティ依存関係の更新

hickory-dns 依存関係の RUSTSEC-2026-0118（クロスゾーン応答での NSEC3 検証の無限ループ）および RUSTSEC-2026-0119（メッセージエンコーディングでの O(n^2) 名前圧縮による CPU 枯渇）が認知され、ワーカーバージョンが更新された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.3)
