## OpenSSL 3.x SSL エラーのリトライ強化

ストリーミング中の追加の OpenSSL 3.x SSL エラーに対するリトライが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## YOLO モードのダウングレード防止

YOLO モードがダウングレードされないよう保護が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## ripgrep バイナリの SEA バンドル

オフラインサポートのため、ripgrep バイナリが SEA（Single Executable Applications）にバンドルされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## ベース URL 環境変数のサポート

`GOOGLE_GEMINI_BASE_URL` および `GOOGLE_VERTEX_BASE_URL` 環境変数が尊重されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## サンドボックスの書き込み権限

明示的な書き込み権限がサンドボックス内のガバナンスファイル保護をオーバーライドできるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## カスタム seatbelt プロファイルの解決

カスタム seatbelt プロファイルが `$HOME/.gemini` から先に解決されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## Bun のデタッチドモード無効化

子プロセスの即時 SIGHUP を防ぐため、Bun のデタッチドモードが無効化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## スキル管理の改善

- スキルクリエイターがスキル抽出エージェントに統合された
- スキル抽出前に繰り返しの証拠が要求されるようになった

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## メモリ管理の刷新

- `memoryManager` フラグが `autoMemory` に分割された
- MemoryManagerAgent がプロンプト駆動の4階層メモリ編集に置き換えられた
- メモリおよびサマリーサービスで jsonl セッションログがサポートされた

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## GitHub カラーブラインドテーマの追加

GitHub のカラーブラインド対応テーマが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## `/new` コマンドの追加

`/clear` のエイリアスとして `/new` コマンドが追加され、コマンド説明が洗練された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## シェルコマンドの改行ラッピング

heredoc の破壊を防ぐため、シェルコマンドのラッピングに改行が使用されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## OSC 777 ターミナル通知

ターミナル通知に OSC 777 が使用されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## `gemini gemma` ローカルモデルセットアップコマンド

ローカルの Gemma モデルを簡単にセットアップする `gemini gemma` コマンドが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## MCP リソースの一覧・読み取りツール

MCP リソースを一覧・読み取りするためのツールが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## .mdx サポート

get-internal-docs ツールで `.mdx` ファイルがサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## トピック更新ナレーションのデフォルト有効化

トピック更新のナレーションがデフォルトで有効になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## ファイル検出の改善

@ レコメンデーションでウォッチャーベースの更新により新規ファイルが検出されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## Vertex AI リクエストルーティング設定

Vertex AI のリクエストルーティングに関する設定が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## 実験的タスクトラッカー機能

実験的なタスクトラッカー機能が導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## セッション永続化のサポート

セッションの永続化がサポートされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## IDE クライアントの動的バージョン

IDE クライアントでハードコードされた '1.0.0' の代わりに動的な CLI バージョンが使用されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## セキュリティ修正

- ワークスペース `.env` による IDE stdio のオーバーライドが禁止された（RCE 脆弱性修正）
- コマンドインジェクションのシェル脆弱性が修正された
- evals、integration-tests、memory-tests の型チェックカバレッジが追加された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## バグ修正

- スラッシュコマンドの IDE リスナーがクリーンアップされた
- `/clear` 時のプランセッション状態がリセットされるようになった
- Cloud Shell ユーザーが PRO_MODEL_NO_ACCESS 実験を使用できるようになった
- OpenTelemetry の float 警告を避けるためスロー描画レイテンシが丸められた
- ネストされたプランディレクトリの重複と相対パスポリシーが修正された
- ignore ファイルのパースで行末が正しく処理されるようになった
- ShellExecutionConfig の展開と ProjectRegistry の保存バックオフが修正された
- ACP セッションでの自動メモリ開始が修正された
- エージェントリフレッシュ時の重複 initialize 呼び出しが削除された
- "/clear (new)" コマンドが修正された
- DevTools のメモリ使用量が削減され、接続が遅延されるようになった
- npm tarball から ripgrep バイナリが除外された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)

## ドキュメント

- インストールと認証のドキュメントがタブ付きレイアウトの MDX に移行された
- system.md のドキュメント内の大文字小文字の不一致が修正された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0)
