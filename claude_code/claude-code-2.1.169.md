## セーフモードの追加

新しい`--safe-mode`フラグおよび`CLAUDE_CODE_SAFE_MODE`環境変数が追加された。すべてのカスタマイズ（CLAUDE.md、プラグイン、スキル、フック、MCPサーバー）を無効にした状態でClaude Codeを起動でき、トラブルシューティングに利用できる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /cdコマンドの追加

新しい`/cd`コマンドが追加され、セッション途中でプロンプトキャッシュを壊さずに作業ディレクトリを変更できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バンドルスキル無効化設定の追加

`disableBundledSkills`設定および`CLAUDE_CODE_DISABLE_BUNDLED_SKILLS`環境変数が追加され、バンドルされたスキル、ワークフロー、組み込みスラッシュコマンドをモデルから非表示にできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 入力ナビゲーションの改善

上下矢印キーが、コマンド履歴にジャンプする前にまず各視覚行を移動するようになり、長い入力行の折り返し時の操作が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /workflowsの即時表示

`/workflows`がターン実行中でも即座に開くようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## TaskCreateの信頼性向上

不正な入力が自動的に修復され、ロードされていないツールのバリデーションエラーにスキーマが含まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## APIキー認証無効時のエラーメッセージ改善

組織がAPIキー認証を無効にしている場合のエラーメッセージが改善され、アクティブなAPIキーの取得元に基づくガイダンスが提供されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## CPU使用率の削減

レスポンスのストリーミング中やスピナーアニメーション中のCPU使用率が削減された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vertex/Foundryのアイドルタイムアウト復元

Vertex/Foundryでデフォルト5分のアイドルタイムアウトが復元され、停滞したストリームが無期限にハングせず中断されるようになった（`API_FORCE_IDLE_TIMEOUT=0`でオプトアウト可能）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションのフラグ保持

バックグラウンドセッションが`--ide`、`--chrome`、`--bare`、`--remote-control`などのフラグをretire→wake間で保持するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## CLAUDE.md長さ警告のスケーリング

「CLAUDE.mdが長すぎる」という警告の閾値がモデルのコンテキストウィンドウに応じてスケーリングされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エンタープライズMCPポリシーの修正

`allowedMcpServers`/`deniedMcpServers`の管理型MCPポリシーが、再接続時、IDE型設定、`--mcp-config`サーバー（インストール直後の初回セッション）、およびリモート設定ロード前に適用されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## コールドスタートの高速化

リモート設定を持たない組織での遅いコールドスタートが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## macOSのUI遅延修正

claude.ai認証情報でログインしているmacOSユーザーで、各ターン開始時に約30-50msのUI遅延が発生する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windowsでのclaude -pの遅延修正

スラッシュコマンド/スキルのスキャン待ちにより`claude -p`が遅くなるまたはハングしているように見える問題が修正された（2.1.161でのリグレッション）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Controlの再接続修正

OAuthトークンのリフレッシュと同時にセッションを再開した際にRemote Controlが「reconnecting」で停止する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WindowsでのGit Credential Managerポップアップ修正

起動時にバックグラウンドgitコマンドがキャッシュされた認証情報なしで実行された際、Git Credential Managerの「Connect to GitHub」ポップアップが表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フッターヒントの表示修正

カスタムステータスラインを使用しているユーザーでフッターヒント（例:「esc to interrupt」）が表示されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントの設定修正

プリウォームされたワーカーにディスパッチされた際、バックグラウンドエージェントがプロジェクトレベルの設定`env`値（例:`ANTHROPIC_MODEL`）を無視する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agents --jsonの修正

`claude agents --json`がブロック中およびディスパッチ直後のバックグラウンドセッションを省略する問題が修正された。完了済みセッションを含める`--all`フラグと、新しい`id`および`state`フィールドが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインキャッシュの修正

WindowsでMCPBプラグインキャッシュが不要に無効化され、再展開が発生する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインロックファイルのクリーンアップ

プラグインの`.in_use` PIDロックファイルが無制限に蓄積する問題が修正された。クラッシュしたセッションの古いマーカーが1日1回クリーンアップされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 信頼されていないプロジェクト設定のセキュリティ修正

信頼されていないプロジェクト設定が、信頼確認なしにOTELクライアント証明書パスを設定できる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)
