## GPT-5.6モデルサポート

GPT-5.6モデルのサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## MCPサーバーリソースのページネーションRPC

MCPサーバーリソースに対するページネーション付き`session.mcp.resources`のread/list/listTemplates RPCが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## --sandboxおよび--no-sandboxフラグの追加

セッション固有のサンドボックス設定を切り替える`--sandbox`および`--no-sandbox`フラグが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## /refineコマンドの追加

粗いプロンプトを整理されたバージョンに書き換える`/refine`コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## /settingsおよび/modelの--repoと--localフラグ

`/settings`と`/model`コマンドに`--repo`および`--local`フラグが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## タイムラインタイムスタンプ表示設定

タイムラインのタイムスタンプの表示・非表示を制御する設定が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## リポジトリレベルの設定ファイルサポート

モデル、エフォート、コンテキストティアを固定するリポジトリレベルの`.github/copilot/settings.json`がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## SDK APIによるライブMCPサーバー管理

実行中のセッション内でライブMCPサーバーを管理するためのSDK APIが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## mcpおよびskillコマンドのエラーメッセージ統一

mcpおよびskillコマンドの失敗時に単一の`Error`プレフィックスが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## web_fetchの必須HTTPSプロキシ対応

`web_fetch`が必須HTTPSプロキシを介して動作するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## 代替サブエージェント実行のキャンセル扱い

代替されたサブエージェント実行が失敗ではなくキャンセルとして扱われるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## GPT-5.6コメンタリーガイダンスの改善

ツール駆動の進捗更新に関するGPT-5.6のコメンタリーガイダンスが改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## タイムラインとツール出力のリンクのクリック対応

タイムラインとツール出力内のマークダウンリンクおよびベアURLがクリック可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## /modelピッカーでのコンテキストウィンドウTab切り替え

`/model`ピッカーでTabキーによるコンテキストウィンドウの切り替えが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## エンタープライズ管理設定の定期リフレッシュ

長時間実行セッションでエンタープライズ管理設定が1時間ごとにリフレッシュされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## ローカルMCPサーバーのサンドボックス表示

ローカルで起動されたMCPサーバーが`/mcp`リストで「(sandboxed)」として表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## 不正カスタムエージェント選択時のエラー表示改善

`--agent`で不正なカスタムエージェントを選択した際に実際のパースエラーが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## プラグインのSHAピンニング

`sha`フィールドによるプラグインの正確なコミットSHAへのピンニングが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## 起動時認証エラーのコマンド案内修正

起動時の認証エラーが正しい`copilot login`コマンドを案内するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## マージセマンティクス設定の編集維持

`/settings`内のマージセマンティクス設定が編集可能な状態を維持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## 管理プラグインのキャッシュ欠損時の再同期

キャッシュが欠損した際に管理プラグインが再同期されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## Ctrl+Yによるプラン・リサーチレポートアクセス

任意のモードからCtrl+Yでプラン・リサーチレポートにアクセス可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## SSH・リモートシェルでのカラースキーム同期

SSHおよびリモートシェルでターミナルカラースキームが同期されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## /chronicleの事前入力クエリ対応

`/chronicle`検索が事前入力クエリを受け付けるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## ツールイベント順序の復元

ツールイベントの順序が復元され、ツール開始後にパーミッションプロンプトが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## Windowsデスクトップトースト通知のクラッシュ修正

Windowsでデスクトップトースト通知によって発生するクラッシュが修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)

## その他の修正・改善

- Gistsタブでの`/search`非表示化
- リモートターミナルでのGitHub Appインストール案内の非表示化
- 最後のアシスタントレスポンスがコマンドエコー後もコピー可能に
- ランタイム再起動時に最後にログインしたユーザーが維持されるように
- `/agent`ピッカーのナビゲーションヒントが選択不可時に非表示に
- no-colorモードでの`/model`ピッカーの別個スクロールバーグリフ表示
- リモートターミナルでのブラウザ起動スキップ
- `/search`と逆検索での矢印キーによる検索モード維持
- ストリーミング中断時の単一キャンセルメッセージ表示
- コンパクトタイムラインビューでの`/pr`テーブル整列
- 空および非ASCII文字のスキル/コマンド名バリデーションエラーの明確化
- セッションバー表示時のフッター選択ハイライト整列
- マーケットプレイスプラグインのgit認証がターミナルプロンプト必要時に即時失敗
- サンドボックス無効化後の保留中のサンドボックスバイパスプロンプト解除

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70)
