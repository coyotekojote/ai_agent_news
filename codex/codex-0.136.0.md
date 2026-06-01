## TUIマークダウンの改善

TUIのマークダウン表示が改善された。WebリンクがOSC 8メタデータでクリック可能になり、狭いテーブルは読みやすいキー/バリュー形式のレコードに切り替わるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## セッションアーカイブ機能

TUI内で`/archive`コマンド、またはCLIで`codex archive`/`codex unarchive`コマンドによるセッションのアーカイブが可能になった。アーカイブされたセッションはリストアされるまでresumeやfork操作から保護される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## App-Server統合の改善

スレッド再開時に初回ターンのページデータが含まれるようになった。MCPサーバーのステータス可視性が向上し、新たに`codex app-server --stdio`モードが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## リモート実行とAPI認証

承認済みOpenAIホストに対する`CODEX_API_KEY`登録がサポートされた。リモートコントロールWebSocketがChatGPTアクセストークンの代わりに短期サーバートークンを使用するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## Windowsサンドボックス

管理者向けのアルファ版`codex sandbox setup --elevated`プロビジョニングパスが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## スタンドアロン画像生成拡張

ネイティブCodex補完パイプラインを通じたスタンドアロン画像生成拡張がフィーチャーゲート付きで追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## 認証・セキュリティの修正

- ChatGPTトークンが5分の有効期限ウィンドウ前にリフレッシュされるようになった
- 再利用されたリフレッシュトークンで汎用クラウドエラーではなく再ログイン要求パスが表示されるようになった

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## コマンド安全性の強化

- `/diff`コマンドがリポジトリ提供のGitヘルパー/フック実行を防止するよう強化された
- PowerShellパーサーの実行が非Windowsホストでブロックされるようになった
- ブラウザ由来のexec-server WebSocketハンドシェイクが拒否されるようになった

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## サンドボックスの信頼性向上

中断後のクリーンアップが改善され、Windowsネットワーク試行の拒否処理が改善された。safe-commandおよびapproval-bypassパスに対して読み取り拒否ルールが適用されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## TUIセッション管理の改善

- resume時にセッショントランスクリプトからプロンプト履歴がシードされるようになった
- マルチラインフック出力が別々の行として表示されるようになった
- Vimノーマルモードの編集が修正された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## App-Serverの改善

- ファイルシステムウォッチャーが後続バッチを正しくデバウンスするようになった
- スタンドアロンWeb検索呼び出しで完了したアクティビティが表示・復元されるようになった

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## Bedrock統合の改善

リージョンが`AWS_REGION`/`AWS_DEFAULT_REGION`にフォールバックするようになった。サポートされていないBedrock GPTサービスティアが広告されなくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## ドキュメントの更新

- Python SDKベータ版のドキュメントとパッケージメタデータが`pip install openai-codex`ガイダンスとともに追加された
- クイックスタート、APIリファレンス、FAQ、サンプルが更新された
- ビルトインツールスキーマの説明でデフォルト値、オプションフィールド、範囲、enumが明確化された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)

## メンテナンス

- MCP依存関係が`rmcp` 1.7.0に更新された
- Amazon Bedrockカタログが GPT-5.5で更新され、OSSエントリが削除された
- Bazel Windowsジョブがcodexランナーに移行された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.136.0)
