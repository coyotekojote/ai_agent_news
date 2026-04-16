## コンテキスト圧縮サービスの正式導入

コンテキストウィンドウ利用を最適化する「Context Compression Service」が正式にリリースされた。コンパクトなツール出力もデフォルトで有効化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.38.0)

## バックグラウンドメモリサービス

スキル抽出のためのバックグラウンドメモリサービスが実装された。メモリの自動設定機能も導入されている。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.38.0)

## サンドボックスのリファクタリング

Linux サンドボックスが ARG_MAX クラッシュを解決するためにリファクタリングされた。Windows サンドボックスの信頼性もネイティブ `__write` 修正により改善された。サンドボックスの承認が正しく永続化・マッチングされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.38.0)

## CLI・UI の強化

- スラッシュコマンドリストが `/skills reload` 後にリフレッシュされるようになった
- デフォルトのローディングフレーズが非表示に変更された
- クリックで展開できるトピック選択機能が追加された
- ツール確認 UI と選択レイアウトが改善された
- 入力プロンプトにスクロールバーが追加された
- `/stats` コマンドにロール別メトリクスが追加された
- `Ctrl+G` キーボードショートカットが追加された（`Ctrl+X` から変更）

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.38.0)

## コア機能の改善

- `complete_task` ツール呼び出しがチャット履歴に記録されるようになった
- サブエージェントのワークスペースディレクトリが AsyncLocalStorage 経由でスコープ化された
- スキルシステム指示がアクティベーション時にサブエージェントプロンプトに注入されるようになった
- フック系システムメッセージが UI に表示されるようになった

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.38.0)

## 設定・構成

- `experimental.adk.agentSessionNoninteractiveEnabled` 設定が追加された
- デフォルト環境変数のサポートが実装された
- Windows/BSD 互換性のため PowerShell 変換が削除され shebang が修正された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.38.0)
