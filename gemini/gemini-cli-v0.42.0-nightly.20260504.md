## /exit コマンドの --delete フラグ追加

`/exit` コマンドに `--delete` フラグが追加され、終了時にセッションを削除できるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## /commands の list サブコマンド追加

`/commands` に `list` サブコマンドが追加され、利用可能なコマンドの一覧表示が可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## 拡張機能のアンインストールエイリアス追加

`/extensions uninstall` のエイリアスとして `delete` が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## 音声モードのマイク統合

音声モードにマイクアイコンが統合され、音声入力のインターフェースが改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## @メンション機能の追加

Gemini ロボットへの @メンション機能が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## ignoreLocalEnv 設定と --ignore-env フラグの追加

`ignoreLocalEnv` 設定と `--ignore-env` フラグが追加され、ローカル環境変数の読み込みを制御できるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## /bug-memory コマンドの追加

`/bug` 機能に `/bug-memory` コマンドが追加され、自動ヒープスナップショットキャプチャによるメモリ診断が可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## Docker マルチステージビルドの改善

Dockerfile がマルチステージビルドに改善され、自己完結型のコンテナ構成が実現された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## API タイムアウトとリトライの改善

デフォルト API タイムアウトが 60 秒に短縮され、undici タイムアウトに対するリトライが有効化された。フォールバックチェーンの処理が改善され、自動モデル選択と明示的選択の maxAttempts が区別されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)

## バグ修正

- AskUser ツールのマークダウンレンダリングで改行のアンエスケープが修正された
- ツールレスポンスから未サポートのマルチモーダルコンテンツタイプがフィルタリングされるようになった
- SkillInboxDialog の代替バッファ表示でレイアウトとスクロールの問題が修正された
- InvalidStream イベントがスローではなくグレースフルに処理されるようになった
- A2A pushMessage の明示的な空ログガードが追加された
- 起動時の重複した拡張機能の警告が抑制されるようになった
- JSON 出力に情報ログが混入する問題が修正された
- readStdin のサイズ制限がバイト長ベースに修正された
- shell 経由の exit_plan_mode 呼び出しが防止された
- サブディレクトリおよびワークツリーでブランチインジケーターが正しく更新されるようになった
- 非 HTTPS プロキシ URL がコンテナ環境でサポートされるようになった

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260504.g37edd1d4d)
