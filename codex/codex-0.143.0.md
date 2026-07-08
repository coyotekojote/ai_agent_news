## リモートプラグインのデフォルト有効化

リモートプラグインがデフォルトで有効になり、カタログ行の表示が充実し、npmマーケットプレイスとの連携が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## macOS・Windowsのシステムプロキシサポート

macOSおよびWindowsにおいて、PACおよびWPAD設定を含むシステムプロキシサポートが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## `codex remote-control pair`コマンドの追加

デーモンから手動ペアリングコードを生成する`codex remote-control pair`コマンドが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## Amazon Bedrock GPT-5.6モデルサポート

Amazon Bedrock GPT-5.6モデル（Sol、Terra、Luna）がファーストクラスの`max`推論エフォートサポートとともに追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## MCPツールのツールサーチデフォルト化

MCPツールがデフォルトでツールサーチを使用するようになり、ChatGPTホスト型MCPサーバーがセッション認証を使用できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## App-serverクライアントの機能拡張

App-serverクライアントが環境の検査、子孫スレッドの一覧表示、履歴のフォークを行えるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## Windows ConPTY入力処理の修正

Windows ConPTYの入力処理が修正され、改行、バックスペース、サンドボックス資格情報のリトライが正しく動作するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## TUIの古いセーフティプロンプトとキャンセルされたレビューの修正

古いTUIセーフティプロンプトとキャンセルされたレビューがMCPの起動完了を妨げる問題が修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## execサーバーオフライン時のリカバリ改善

execサーバーが一時的にオフラインになった際のリカバリが改善され、remote-controlトークンリフレッシュのリトライストームが防止された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## シャットダウン時のトランスクリプト保持修正

シャットダウン時にトランスクリプトテキストとターミナルロールアウトイベントが保持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## WebSocketリクエスト成功率の改善

レスポンスメタデータの比較を無視することで、インクリメンタルWebSocketリクエストの成功率が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## インストーラーのGitHub APIレートリミット対応

リリースメタデータの再利用により、GitHub APIレートリミットによるインストーラー失敗が削減された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## UUID7スレッド・ターンIDのドキュメント化

UUID7によるスレッドおよびターンIDがドキュメント化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)

## セキュリティアップデート

OpenSSLが3.6.3に更新され、Hono、fast-uri、quick-xml、crossbeam-epoch（RUSTSEC-2026-0204）のセキュリティアドバイザリに対応するアップデートが行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.143.0)
