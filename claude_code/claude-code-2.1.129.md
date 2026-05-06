## --plugin-url フラグの追加

`--plugin-url <url>` フラグが追加され、URL からプラグインの `.zip` アーカイブを取得して現在のセッションで使用できるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## 同期出力の強制有効化

`CLAUDE_CODE_FORCE_SYNC_OUTPUT=1` 環境変数が追加され、自動検出が機能しないターミナル（例: Emacs `eat`）で同期出力を強制的に有効化できるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## パッケージマネージャーの自動更新

`CLAUDE_CODE_PACKAGE_MANAGER_AUTO_UPDATE` 環境変数が追加され、Homebrew または WinGet インストール環境でバックグラウンドでアップグレードコマンドを実行し、再起動を促すようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## プラグインマニフェストの experimental 宣言

プラグインマニフェストの `themes` と `monitors` は `"experimental": { ... }` 配下で宣言する形式に変更された。トップレベルの宣言は引き続き動作するが、`claude plugin validate` で警告が表示される。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## Gateway モデル検出のオプトイン化

Gateway `/v1/models` の `/model` ピッカー向け検出が `CLAUDE_CODE_ENABLE_GATEWAY_MODEL_DISCOVERY=1` によるオプトインに変更された（2.1.126〜2.1.128 では自動的に有効だった）。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## Ctrl+R 履歴ピッカーのデフォルト変更

Ctrl+R 履歴ピッカーがデフォルトで全プロジェクトの全プロンプトを検索するようになり、2.1.124 以前の動作に戻った。Ctrl+S で現在のプロジェクトまたはセッションに絞り込み可能。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## サードパーティデプロイのスピナーヒント改善

サードパーティデプロイ（Bedrock、Vertex、Foundry、`ANTHROPIC_BASE_URL` ゲートウェイ）でファーストパーティの Anthropic サーフェスを指すスピナーヒントが表示されなくなった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## skillOverrides 設定の動作修正

`skillOverrides` 設定が正しく動作するようになった。`off` でモデルと `/` から非表示、`user-invocable-only` でモデルからのみ非表示、`name-only` で説明を折りたたみ。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## PR/MR カウントメトリクスの改善

`claude_code.pull_request.count` OTel メトリクスがシェルコマンドだけでなく MCP ツール経由で作成された PR/MR もカウントするようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## ポリシー拒否エラーメッセージの改善

ポリシー拒否のエラーメッセージに API Request ID が含まれるようになり、サポートデバッグが容易になった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)

## バグ修正

- 認識されない 400 ステータスコードの API エラーで生の JSON が表示される問題が修正され、適切なエラーメッセージが表示されるようになった
- `/clear` 後にターミナルタブタイトルがリセットされない問題が修正された
- `/rename` で設定したセッションタイトルチップがパーミッションダイアログ等の表示中に消える問題が修正された
- サブエージェント実行中にプロンプト下のエージェントパネルが非表示になる問題が修正された（2.1.122 のリグレッション）
- 外部エディタハンドオフ（Ctrl+G）でプロンプト上の会話履歴が空白になる問題が修正された
- `/context` がレンダリングされた ASCII 可視化グリッドを会話に出力し、呼び出しごとに約 1.6k トークンを浪費する問題が修正された
- `/agents` ライブラリリストの矢印キーナビゲーションで、リストがビューポートを超えた場合にハイライトされたエージェントが見えなくなる問題が修正された
- `/branch` の成功メッセージに `/resume` 用の新しいブランチのセッション ID が含まれない問題が修正された
- フルスクリーンモードでキーキャップ/ZWJ/スキントーン絵文字を含む太字ヘッダーの末尾文字が失われる問題が修正された
- エンタープライズ/チームユーザーで保存された OAuth 認証情報に `user:inference` スコープがない場合にサーバー管理設定ポリシーが適用されない問題が修正された
- スリープ復帰後の OAuth リフレッシュレースにより、実行中の全セッションがログアウトされる問題が修正された
- 1 時間のプロンプトキャッシュ TTL が黙って 5 分にダウングレードされる問題が修正された
- `/clear` やコンパクション後に `/effort` や `/model` を変更した際にキャッシュミス警告が誤って表示される問題が修正された
- `Bash(mkdir *)`、`Bash(touch *)` などの許可ルールがプロジェクト内パスに対して適用されない問題が修正された
- `deniedMcpServers` パターンで `*://` スキームワイルドカードが大文字小文字混在のホスト名にマッチしない問題が修正された
- `--debug` 時にボイスモード中に無害な WebSocket 警告がエラーとしてログ出力される問題が修正された
- [VSCode] `/clear` で会話コンテキストと表示されたトランスクリプトがクリアされない問題が修正された

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.129)
