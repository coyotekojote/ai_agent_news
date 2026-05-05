## CLI 起動の高速化

認証がバックグラウンドで解決される間に UI が即座にレンダリングされるようになり、CLI の起動が高速化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## シェル補完の自動インストール

シェル補完（bash、zsh、fish）が初回実行時に自動インストールされ、`copilot update` 後に自動更新されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## スラッシュコマンドのタブ補完改善

引数付きのスラッシュコマンドをタブ補完した際に末尾のスペースが自動追加されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## 実験的 MCP Tasks サポート

`taskSupport: 'required'` を持つ MCP ツールがノンブロッキングのバックグラウンドエージェントとして実行され、`list_agents` と `read_agent` で追跡可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## プロンプトモードでの拡張機能読み込み

拡張機能がプロンプトモードで読み込まれるようになった。ユーザー拡張機能はデフォルトで読み込まれ、プロジェクト拡張機能は環境フラグが必要。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## --attachment フラグの追加

`-p/--prompt` を使用した非インタラクティブモードで `--attachment` フラグが追加され、ファイルを初期プロンプトに添付できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## プロンプトでの Markdown レンダリング

ask user プロンプトで Markdown フォーマットが正しくレンダリングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## スラッシュコマンドピッカーの検索改善

スラッシュコマンドピッカーが説明文も検索対象とし、マッチした文字にアンダーラインが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## メモリスコープの表示

メモリ保存時の確認プロンプトにリポジトリスコープかユーザースコープかが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## ストリーミングアニメーションのパフォーマンス改善

低速またはビジーなシステムでもストリーミングテキストとシマーアニメーションがスムーズに動作するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## リモートセッションエラーの改善

接続エラー時にログイン済みアカウント情報とカスタマイズされたトラブルシューティングガイダンスが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## Git SSH プラグインマーケットプレイスサポート

プラグインマーケットプレイスで Git SSH URL が正しく機能するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)

## バグ修正

- Windows でウイルス対策やファイルシステムロックによる一時的な EPERM エラーでパッケージ展開がクラッシュする問題が修正された
- アシスタント応答に不要なシステム通知 XML タグが含まれなくなった
- 大出力ガイダンスが設定された grep ツール名を正しく参照するようになった
- SQL todo タイムラインエントリの表示精度が向上した
- ファジーまたは位置ずれしたエディットブロックからの回復が改善され、ファイル編集の信頼性が向上した
- `./` パスでの @メンション補完が正しく動作するようになった
- 補完候補でプロジェクトファイルがワークスペースルートより前に表示されるようになった
- Windows で Node 24.x の V8 クラッシュが回避された
- セッションファイル内の Unicode 行区切り文字が正しく読み込まれるようになった
- 推論エフォートピッカーのヒントテキストの表示間隔が修正された

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.41)
