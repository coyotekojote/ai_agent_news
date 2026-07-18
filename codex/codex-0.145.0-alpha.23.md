## 未使用のTUIコラボレーションモードインジケーター削除

未使用の`PairProgramming`および`Execute`フッターバリアントが削除された。

[参考リンク](https://github.com/openai/codex/pull/33872)

## コラボレーションモード命令のワールドステート追跡

コラボレーションモードが永続化されたワールドステートセクションとしてモデル化された。

[参考リンク](https://github.com/openai/codex/pull/33876)

## CLIを外部エージェント設定インポートソースとして報告

TUI起動リクエストのインポートソース識別が修正された。

[参考リンク](https://github.com/openai/codex/pull/33883)

## スレッドMCP接続のMcpRuntimeへの集約

アトミックな接続セット更新のためのスレッド所有ランタイムが追加された。

[参考リンク](https://github.com/openai/codex/pull/33889)

## ロールアウトメタデータ読み取りのヘッダー限定

メタデータ抽出がロールアウト全体ではなくヘッダーのみをスキャンするよう最適化された。

[参考リンク](https://github.com/openai/codex/pull/33892)

## リアルタイム会話状態のワールドステート追跡

リアルタイムステータスが永続化されたワールドステートセクションとして表現されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33893)

## スレッドティアダウン用SessionEndフックの追加

グレースフルなスレッドシャットダウンのための`SessionEnd`フックイベントが導入された。

[参考リンク](https://github.com/openai/codex/pull/33895)

## プラグインインストールインタースティシャル要件の公開

プラグインレスポンスに`mustShowInstallationInterstitial`メタデータが追加された。

[参考リンク](https://github.com/openai/codex/pull/33896)

## ChatGPTブランドDesktopアプリビルドのサポート

macOS/WindowsでChatGPTとCodex両方のブランディング検出が有効化された。

[参考リンク](https://github.com/openai/codex/pull/33901)

## メッセージ履歴のバウンド付きバッチルックアップ追加

サイズ制限付きのカーソルベースページネーションが履歴エントリに実装された。

[参考リンク](https://github.com/openai/codex/pull/33902)

## リアルタイムV3ハンドオフのレスポンスチャネルルーティング

V3セッションレスポンスルーティングのための`codexResponseHandoffMode`が追加された。

[参考リンク](https://github.com/openai/codex/pull/33903)

## 逆検索時の永続履歴バッチ読み取り

逆検索がエントリごとのルックアップではなくバッチ読み取りを使用するよう最適化された。

[参考リンク](https://github.com/openai/codex/pull/33905)

## リモートエグゼキューターでのマネージドネットワークプロキシ起動

リモート実行のためのエグゼキューターローカルプロキシリスナーが実装された。

[参考リンク](https://github.com/openai/codex/pull/33906)

## ページネーションスレッドの出現検索追加

UTF-16範囲を持つ実験的な`thread/searchOccurrences`メソッドが作成された。

[参考リンク](https://github.com/openai/codex/pull/33907)

## シェア更新によるプラグイン公開の許可

プラグイン共有APIで`LISTED`ディスカバラビリティが受け入れられるようになった。

[参考リンク](https://github.com/openai/codex/pull/33908)
