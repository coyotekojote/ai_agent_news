## ゲートウェイ経由のモデルピッカー対応

`ANTHROPIC_BASE_URL` が Anthropic 互換ゲートウェイを指す場合、モデルピッカーがゲートウェイの `/v1/models` エンドポイントからモデル一覧を取得するようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## プロジェクト状態の完全削除コマンド追加

`claude project purge [path]` コマンドが追加され、プロジェクトの Claude Code 状態（トランスクリプト、タスク、ファイル履歴、設定エントリ）を一括削除できるようになった。`--dry-run`、`-y/--yes`、`-i/--interactive`、`--all` オプションに対応している。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## --dangerously-skip-permissions の保護パス拡張

`--dangerously-skip-permissions` が `.claude/`、`.git/`、`.vscode/`、シェル設定ファイルなどの保護パスへの書き込みプロンプトもバイパスするようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## OAuth 認証のターミナル貼り付け対応

`claude auth login` でブラウザコールバックが localhost に到達できない場合（WSL2、SSH、コンテナ環境）、ターミナルに OAuth コードを貼り付けて認証できるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## スキル起動の OpenTelemetry イベント改善

`claude_code.skill_activated` OpenTelemetry イベントがユーザー入力のスラッシュコマンドに対して発火するようになり、新たに `invocation_trigger` 属性が追加された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## オートモードのスピナー改善

オートモードでパーミッションチェックが停滞した際、スピナーが赤色に変化するようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## ホスト管理デプロイメントのアナリティクス設定修正

ホスト管理デプロイメントで Bedrock/Vertex/Foundry 使用時にアナリティクスが自動無効化されなくなった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## Windows PowerShell 対応の改善

PowerShell 7 の検出が改善され、Microsoft Store、PATH なしの MSI、.NET グローバルツールインストールに対応した。また、Bash がデフォルトではなく PowerShell がプライマリシェルとして扱われるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## Read ツールのマルウェア評価リマインダー削除

Read ツールのファイルごとのマルウェア評価リマインダーが削除され、誤拒否の原因が解消された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## セキュリティ修正

`allowManagedDomainsOnly` / `allowManagedReadPathsOnly` が、より高優先度のマネージド設定ソースに `sandbox` ブロックがない場合に無視される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)

## バグ修正

- 2000px を超える画像の貼り付けでセッションが破損する問題が修正され、貼り付け時に自動縮小されるようになった
- 「OAuth not allowed for organization」エラー時にログイン画面が表示される問題が修正された
- 低速/プロキシ接続および IPv6 専用 devcontainer での OAuth ログインタイムアウトが修正された
- 並行クレデンシャル書き込みで有効な OAuth リフレッシュトークンが消去されるレースコンディションが修正された
- API リトライカウントダウンが「0s」で停止する問題が修正された
- Mac スリープ復帰後の「Stream idle timeout」エラーが修正された
- バックグラウンド/リモートセッションで長時間のモデル思考中に「Stream idle timeout」で中断される問題が修正された
- アシスタントが思考完了後に出力を表示しないハングが修正された
- Cursor および VS Code 1.92-1.104 の統合ターミナルでのトラックパッドスクロール速度の問題が修正された
- 手動サーバーが needs-auth 状態で停滞する場合に claude.ai MCP コネクタが抑制される問題が修正された
- Windows のノーフリッカーモードで日本語/韓国語/中国語テキストが文字化けする問題が修正された
- `Ctrl+L` がプロンプト入力をクリアする問題が修正され、画面再描画のみに変更された
- `context: fork` を持つスキルおよびサブエージェントで初回ターンにデファードツールが利用できない問題が修正された
- `--channels` で起動したインタラクティブセッションでプランモードツールが利用できない問題が修正された
- `/plugin` のアンインストール時に「Enabled」と表示される問題が「Uninstalled」に修正された
- リンターが多数のファイルに触れた際のファイル変更リマインダーのサイズが制限された
- `/remote-control` リトライが「connecting...」で停滞する問題が修正された
- リモートコントロール初回接続失敗時にエラー理由が表示されない問題が修正された
- Windows でクリップボード書き込みがプロセスコマンドライン引数に露出する問題が修正された
- PowerShell ツールで `--` が `--%` ストップパーシングトークンとして誤検出される問題が修正された
- Agent SDK でモデルが並行ツールコールバッチ内で不正なツール名を出力した際のハングが修正された

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.126)
