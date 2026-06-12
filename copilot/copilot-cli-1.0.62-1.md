## YOLOインジケーターの追加

フッターに「YOLO」（全許可）インジケーターが追加され、カスタム`statusLine.command`ステートに対応した。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## Issues/PRタブでのGitHub検索機能

Issues/PRタブで「/」キーを押すことでサーバーサイドフィルタリングによるGitHub検索が利用可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## セッションスコープの拡張機能とキャンバス

セッションスコープの拡張機能とキャンバスが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## SDK クライアントのセッションメモリ設定

SDKクライアントが`session.create`および`session.resume`メソッドでセッションメモリを設定できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## 企業プロキシのKerberos/SPNEGO認証対応

Kerberos/Negotiate（SPNEGO）を使用した企業フォワードプロキシ経由の自動認証がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## /diffビューのファイルツリーサイドバーとインラインコメントエディター

`/diff`ビューにファイルツリーサイドバーとインラインコメントエディターが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## ワークツリー作成の改善

Issue/PRの詳細表示から「W」キーでワークツリーを作成できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## スラッシュコマンドのスケジューリング強化

`/every`および`/after`コマンドでスラッシュコマンドのスケジューリングが可能になった（例：「/every 1d /chronicle standup」）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## モデルピッカーの改善

モデルピッカーが現在選択中のモデルのタブを開いて表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## シェルコマンドの軽量プロセス実行

シェルコマンドの実行が疑似ターミナルの代わりに軽量なプロセススポーンを使用するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## WCAG AAアクセシビリティカラーコントラスト

GitHubテーマでWCAG AAアクセシビリティ基準に準拠したカラーコントラストが実装された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## ブランチ・HEAD検出の高速化

ウォームセッションでのブランチおよびHEAD検出が高速化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## max_output_tokensの修正

BYOKレスポンスプロバイダーで`max_output_tokens`が正しく適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## MCPサーバー名のネームスペースマッピング修正

ドットやスラッシュを含むMCPサーバー名がResponses APIの有効なネームスペースに正しくマッピングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## Windowsでのエディターコマンド起動修正

`code-insiders --wait`のようなエディターコマンドがWindows上で正しく起動するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## シンボリックリンクディレクトリのスキル読み込み修正

シンボリックリンクされたディレクトリからのスキル読み込みが修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## 画像処理の安定性向上

オーバーサイズのインライン画像が適切に処理されるようになり、セッション失敗が防止された。ビジョン無効時の画像添付がセッション履歴を破損しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## バックグラウンドシェルタスクの持続性修正

バックグラウンドシェルタスクがターン完了後も維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## ネストされたカスタムエージェントの検出

リポジトリのサブディレクトリにあるカスタムエージェントが起動時に検出されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## ツールパーミッションプロンプトの重複解消

ツールパーミッションプロンプトによる重複リクエストが解消された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## テーマ変更時のターミナルカラー更新

セッション中にテーマを変更した際にターミナルカラーがリアルタイムで更新されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)

## その他の修正

サンドボックスツールのmxc-sdkホスト環境での読み込みが修正された。Viewツールのトランケーション制限が修正された（20KB対50KB）。ワークスペースMCPサーバーの再起動ループが防止された。BYOKプロバイダーでのカスタムエージェントのモデル割り当てが維持されるようになった。コンテンツポリシーエラーのリカバリーが実装された。Autopilotリレーセッション機能と`/plan`プロンプト表示が修正された。WindowsでGitコマンド実行時のコンソールウィンドウのフラッシュが解消された。ネストされたサブエージェントの同時実行制限がターミナルブロックなしで強制されるようになった。完全修飾タグ参照のプラグインインストールがサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62-1)
