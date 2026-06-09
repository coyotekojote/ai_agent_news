## /appコマンドによるDesktopハンドオフ

`/app`コマンドがmacOSおよびWindowsでCLIセッションからCodex Desktopへのハンドオフをサポートするようになった。Windowsのワークスペース起動時に手動プロンプトで止まらず直接Desktopを開けるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## ローカル画像添付のファイルパス公開

ローカル画像の添付やスタンドアロン画像生成で保存先ファイルパスがモデルに公開されるようになり、フォローアップ編集やファイル参照の信頼性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## 推論エフォート選択の強化

TUIにAltバインディングが利用できないターミナル向けのフォールバックショートカットが追加された。モデル定義のエフォートレベルが公表順に表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## アカウントトークン使用量の読み取り

App-server統合でアカウントトークンの使用量を読み取れるようになった。Codex認証がCLIおよびapp-serverフローでv2パーソナルアクセストークンをサポートするようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## プラグイン自動化の拡充

add/removeおよびマーケットプレイスコマンドが`--json`出力をサポートするようになった。プラグインリストのJSONにマーケットプレイスソース情報が含まれ、デフォルトプロンプト、リモートMCPサーバー、利用不可アプリテンプレートが公開されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## ゴールワークフローの改善

`/goal edit`でのマルチライン貼り付けが途中で送信されなくなった。アイドル自動ターンがPlanモードから除外され、ターミナルターン失敗後にゴールが自動継続しなくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## フォークスレッドの名前保持

フォークされたスレッドが、元の最初のプロンプト名にフォールバックする代わりにユーザーがリネームしたタイトルを保持するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## TUI表示の改善

ストリーミング中の余分な空白が排除された。キャンセルされたプロンプトがカーソルを末尾に置いた状態で再開されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## 設定エラーレポートの改善

TUI設定の書き込み失敗時に根本原因が表示されるようになり、バリデーション問題や読み取り専用ファイルシステムの問題が診断しやすくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## 起動の安定性向上

`/usr/bin/bash`シェルフォールバックのサポート、Linuxプロキシソケットパスの短縮化、期限切れOAuth連携MCP認証情報の事前リフレッシュが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## ワークスペース指示の読み込み改善

リモートやシンボリックリンクされたワークスペースでの読み込み精度が向上し、`AGENTS.md`ファイルの検出が一貫するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## TUI起動の最適化

プラグイン検出結果が再利用され、クリティカルパスではフックメタデータのみが読み込まれるようになった。`resume --last`が状態DBを通じて最新の一致セッションを最初に検索するようになり、大規模なローカル履歴での復元が高速化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)

## ストリーム処理の高速化

大規模なMCP/Ollamaストリームの処理が高速化され、最適化されたバイトスキャンにより長いメッセージ履歴が加速された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0)
