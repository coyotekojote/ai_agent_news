## MCPファイルアップロードの環境ファイルシステム経由化

MCPファイルアップロードが環境ファイルシステムを通じてルーティングされるようになった。

[参考リンク](https://github.com/openai/codex/pull/27923)

## app-serverのターゲットネイティブ環境cwd保持

app-serverがターゲットネイティブ環境のcwdを正しく保持するようになった。

[参考リンク](https://github.com/openai/codex/pull/28146)

## /usageのレート制限リセット表示

`/usage` にレート制限のリセット時間の表示が追加された。

[参考リンク](https://github.com/openai/codex/pull/28154)

## コードモード出力の切り詰め警告

コードモードの出力が切り詰められた際に明確な警告が表示されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28467)

## リモートサンドボックスホスト名ルックアップの遅延評価

リモートサンドボックスのホスト名ルックアップが遅延評価されるようになり、設定読み込みのパフォーマンスが向上した。

[参考リンク](https://github.com/openai/codex/pull/28542)

## C++モジュールファイルのハイライト修正

C++モジュールファイル（`.cppm`等）のシンタックスハイライトが修正された。

[参考リンク](https://github.com/openai/codex/pull/28554)

## PathURI処理の改善

PathURIのシリアライズ互換性、パス移行の不変条件記録、モデル生成パスとレガシーアプリパスタイプの明確化が行われた。

[参考リンク](https://github.com/openai/codex/pull/28595)
