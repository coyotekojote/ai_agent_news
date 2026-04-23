## ripgrep バイナリの SEA バンドル

ripgrep バイナリが SEA（Single Executable Application）にバンドルされ、オフライン環境でのサポートが強化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## MCP リソースツールの追加

MCP リソースの一覧表示と読み取りを行うツールが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## GitHub カラーブラインドテーマ

色覚多様性に対応した GitHub カラーブラインドテーマが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## スキル抽出エージェントの統合

skill-creator がスキル抽出エージェントに統合され、再発エビデンス要件が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## MemoryManager のリファクタリング

MemoryManagerAgent が 4 段階のプロンプト駆動型編集に置き換えられた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## Gemma ローカルモデルセットアップ

`gemini gemma` コマンドによる合理化されたローカルモデルセットアップが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## ターミナル通知

OSC 777 標準によるターミナル通知が実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## Vertex AI リクエストルーティング

Vertex AI リクエスト管理の設定が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## `/new` コマンドエイリアス

`/clear` のショートカットとして `/new` コマンドが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## JSONL セッションログのサポート

メモリおよびサマリーサービスが JSONL 形式のセッションログに対応した。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## MDX ドキュメントサポート

内部ドキュメントツールが MDX ファイルを認識するよう拡張された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## セキュリティ改善

- IDE の stdio オーバーライドがワークスペース `.env` 経由で行われることを防止する RCE 対策が実施された
- シェルコマンド実行のインジェクション防止が強化された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)

## バグ修正

- OpenSSL 3.x でのストリーミング中の追加 SSL エラーに対するリトライ処理が修正された
- YOLO モードのダウングレード動作が修正された
- `GOOGLE_GEMINI_BASE_URL` および `GOOGLE_VERTEX_BASE_URL` 環境変数が正しく反映されるようになった
- IDE リスナーのクリーンアップに関するスラッシュコマンドの問題が解消された
- セッション永続化機能が有効化された
- テーマダイアログのラベルレンダリングが全テーマオプションで修正された
- heredoc の改行ベースラッピングによるシェルコマンド保持が修正された
- Bun のデタッチモードが無効化され、子プロセスのシグナル問題が解消された
- `/clear` 時のプランセッション状態リセットが修正された
- ACP セッションでの自動メモリ初期化が保証された
- API キーバリデーションでドットが許可されるようになった
- プレビューテーマのダイアログアンマウント時のリバージョンが修正された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.40.0-preview.2)
