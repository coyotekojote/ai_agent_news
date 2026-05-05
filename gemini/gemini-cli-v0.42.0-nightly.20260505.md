## LaTeX 出力の Unicode レンダリング

TUI で LaTeX スタイルの出力が Unicode としてレンダリングされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260505.g8f0edcd64)

## リアルタイム音声モードのプライバシー警告

Gemini Live バックエンドの音声機能に対してプライバシーおよびコンプライアンスに関する UX 警告が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260505.g8f0edcd64)

## Auto Memory インボックスフロー

Auto Memory インボックスフローが導入され、canonical-patch コントラクトがサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260505.g8f0edcd64)

## /bug-memory コマンドの追加

`/bug` コマンドに `/bug-memory` が追加され、自動ヒープスナップショットキャプチャによるメモリ診断が可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260505.g8f0edcd64)

## /agents refresh のログ改善

`/agents refresh` コマンドのログ出力が改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260505.g8f0edcd64)

## SDK の JSDoc 追加

SDK のエクスポートされたインターフェースと型に JSDoc が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260505.g8f0edcd64)

## Docker マルチステージビルドの改善

Dockerfile が自己完結型マルチステージビルドに再構成された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260505.g8f0edcd64)

## バグ修正

- スキル同意ダイアログがリロード前にクリアされるようになった
- 子プロセスのフォールバックで exit ではなく close イベントが使用されるようになった
- ツールレスポンスから未サポートのマルチモーダルタイプがフィルタリングされるようになった
- AskUser ツールのマークダウンで改行が正しくアンエスケープされるようになった
- SkillInboxDialog が代替バッファで正しくフィットしスクロールするよう修正された
- ホームディレクトリ警告のチェックが os.homedir() を使用するよう修正された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260505.g8f0edcd64)
