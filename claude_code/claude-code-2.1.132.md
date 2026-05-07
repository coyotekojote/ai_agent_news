## 環境変数の追加

Bash ツールのサブプロセス環境に `CLAUDE_CODE_SESSION_ID` 環境変数が追加された。また、`CLAUDE_CODE_DISABLE_ALTERNATE_SCREEN=1` を設定することでフルスクリーンレンダラーをオプトアウトできるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## 画像ペースト時のフッターヒント

Ctrl+V で画像をペーストする際に「Pasting…」というフッターヒントが表示されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## シグナル処理とターミナル復元の修正

外部 SIGINT がグレースフルシャットダウンを実行しない問題が修正され、ターミナルモードが正しく復元されるようになった。ターミナルが閉じられたり SSH が切断された際の未キャッチ例外も修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## セッション再開時の修正

`--resume` でツールエラーメッセージの絵文字切り捨てにより失敗する問題が修正された。また、`--permission-mode` フラグがプランモードセッションの再開時に無視される問題も修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## フルスクリーンモードの修正

ラップトップのスリープ/復帰後や Ctrl+Z/fg 後にフルスクリーンモードが空白画面になる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## テキスト表示・入力の修正

インド系結合文字や ZWJ 絵文字のカーソル位置の問題、vim オペレーターが分解済み（NFD）アクセント文字を破損する問題が修正された。`/` で始まるテキストのペーストが無視される問題や、フォーカスイベントとブラケットペーストが干渉して不要なエスケープシーケンスが出力される問題も修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## IDE ターミナルでのスクロール修正

Cursor および VS Code 1.92–1.104 でマウスホイールスクロールが速すぎる問題、JetBrains IDE 2025.2 ターミナルでのスクロールホイール処理の問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## スラッシュコマンド関連の修正

`/usage` の Ctrl+S が Linux/X11 クリップボードコピーでハングする問題、`/terminal-setup` が Windows Terminal で矛盾したエラーを表示する問題、`/effort` ピッカーが `CLAUDE_CODE_EFFORT_LEVEL` 環境変数を反映しない問題、`/status` が一部ユーザーに対して誤ったデフォルトモデルを表示する問題が修正された。スラッシュコマンドの自動補完ポップアップが約3〜5コマンドに制限されていた問題も修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## ステータスラインの修正

ステータスラインの `context_window` トークンカウントが累積値を表示していた問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## キーボード入力の修正

macOS ターミナルで「Option as Meta」が無効な場合に Alt+T（思考トグル）が動作しない問題、Windows でバックグラウンドセッションを再度開いた後にキーボード入力が無反応になる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## MCP 関連の修正

非プロトコル MCP サーバー出力による無制限メモリ増加（10GB+ RSS）の問題が修正された。MCP サーバーが 0 ツールの代わりに「tools fetch failed」と表示される問題、未認可の claude.ai MCP コネクタが「needs auth」ではなく「failed」と表示される問題も修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)

## Bedrock / Vertex の修正

`ENABLE_PROMPT_CACHING_1H` 設定時に Bedrock および Vertex で 400 エラーが発生する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.132)
