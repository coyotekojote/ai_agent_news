## 自動アップデートのチャンネル安定性保護

自動アップデートがより不安定なチャンネルに切り替わることが防止されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## SEA 対応の NODE_OPTIONS パス

リランチ時に NODE_OPTIONS を経由してノード引数が渡されるようになり、SEA（Single Executable Application）がサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## ターミナルキーパッド Enter シーケンス対応

DECKPAM キーパッドの Enter シーケンスが正しくハンドリングされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## Gemma 4 モデルのデフォルト有効化

Gemini API 経由で Gemma 4 モデルがデフォルトで有効化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## 音声モードの UI 改善

音声モードにマイクアイコンとウェーブアニメーションが追加され、音声転写がカーソル位置に挿入されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## @メンション機能の追加

Gemini ロボットへの @メンション機能が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## /exit --delete フラグの追加

`/exit` コマンドに `--delete` フラグが追加され、終了時にセッションを削除できるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## /commands list サブコマンドの追加

`/commands` に `list` サブコマンドが追加され、利用可能なコマンドの一覧表示が可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## 拡張機能の delete エイリアス追加

`/extensions uninstall` のエイリアスとして `delete` が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## ignoreLocalEnv 設定と --ignore-env フラグ

`ignoreLocalEnv` 設定と `--ignore-env` フラグが追加され、ローカル環境変数の読み込みを制御できるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## /bug-memory コマンドの追加

`/bug` に `/bug-memory` コマンドが追加され、自動ヒープスナップショットキャプチャによるメモリ診断が可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## API タイムアウトとリトライの改善

デフォルト API タイムアウトが 60 秒に短縮され、リトライが有効化された。フォールバックチェーンの処理が改善され、`ERR_STREAM_PREMATURE_CLOSE` エラーでもリトライされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## Ghostty/raw モードの OAuth フロー修正

Ghostty/raw モードでの OAuth フロー中の偽キャンセル問題が解決された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## サブエージェントの承認モード認識

サブエージェントがアクティブな承認モードを認識するようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## Vertex AI 使用時の Cloud Shell 環境変数保護

Cloud Shell で Vertex AI 使用時に `GOOGLE_CLOUD_PROJECT` が上書きされなくなった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## セキュリティ強化

Inquiry の制約が強化され、未承認の変更が防止されるようになった。また、`logPrompts` フラグによる機密フィールドのログ制御が尊重されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)

## バグ修正

- Escape キーが入力バッファをクリアしないよう修正された
- MCP クライアントが拡張機能停止時に正しく切断されるようになった
- A2A pushMessage の明示的な空ログガードが追加された
- InvalidStream イベントがスローではなくグレースフルに処理されるようになった
- セッション再開時にセッションスコープの状態がリセットされるようになった
- GrepTool の大文字小文字の一貫性が修正された
- 非 HTTPS プロキシ URL がコンテナ環境でサポートされるようになった
- GEMINI.md パスがディレクトリの場合にサイレントスキップされるようになった
- ツール承認のレースコンディションが修正された
- 設定ダイアログの境界線がクリップされないよう maxHeight を使用して修正された
- shell ツールヘッダーが Ctrl+O で折り返されるようになった
- ブランチインジケーターがサブディレクトリおよびワークツリーで正しく更新されるようになった
- readStdin のサイズ制限がバイト長ベースに修正された
- shell 経由の exit_plan_mode 呼び出しが防止された
- 情報ログが JSON 出力に混入する問題が修正された
- 起動時の重複した拡張機能警告が抑制された
- WSL でのプラットフォーム固有の undo/redo とスマートバブリングが改善された
- InvalidStream イベント時の「System: Please continue.」インジェクションが削除された
- partialConfig での冗長な GEMINI.md 読み込みがスキップされるようになった
- 圧縮中にメッセージのキューイングが許可されるようになった

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-preview.0)
