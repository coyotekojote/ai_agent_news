## 自動アップデートの安定性チャネル降格防止

自動アップデートがより不安定なチャネルに切り替わることが防止された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26132)

## settings.json の環境変数でブール値・数値キャストに対応

settings.json の環境変数でブール値と数値のキャストがサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26118)

## SEA 対応の Node 引数パス

リランチ時に `NODE_OPTIONS` 経由で Node 引数が渡されるようになり、SEA（Single Executable Application）がサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26130)

## サブエージェントパースの OAuth フィールド対応

サブエージェントパースで不足していた OAuth フィールドのサポートが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26141)

## DECKPAM キーパッド Enter シーケンスのターミナル処理

ターミナルで DECKPAM キーパッドの Enter シーケンスが正しく処理されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26092)

## バグ修正

- 一時的なエラーが誤ってターミナル（致命的）としてマークされる問題が修正された
- 非文字列のモデルフラグが解決時に正しく処理されるようになった
- ENOTDIR のエラーメッセージが追加された
- SessionEnd フックからの ACP stdout 汚染が防止された
- DevTools アクティビティロガーで Request ヘッダーが保持されるようになった
- 拡張機能ベースの MCP クライアントが `stopExtension` 時に切断されるようになった

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260429.g6d9911393)

## リポジトリ管理改善ボットの実装

時系列メトリクス分析とリポジトリ管理改善提案を行うボットが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25945)
