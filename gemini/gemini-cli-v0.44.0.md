## EISDIRエラーの解消

仮想ドライブやその他のストレージシステムでのファイル処理中に発生するEISDIRエラーが解消された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## 自動モデル解決の修正

`hasAccessToPreview`を使用した自動モデル解決が修正され、制限付きプレビューモデルに対する安定したフォールバックが確保された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## https-proxy-agentの外部化

`https-proxy-agent`が外部化され、グローバルfetchディスパッチャーおよびネットワークベースMCPサーバーで`NO_PROXY`環境変数が尊重されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## シェル出力のスロットリング

シェルテキスト出力のスロットリングとライブUIバッファの制限が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## 型安全性の向上

unsafe-return抑制が厳密な型バリデーションにより排除された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## コンテキストファイルの動作変更

コンテキストファイルが置換ではなく追記方式に変更された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## キーチェーン認証の拡張

キーチェーン認証が`--list-sessions`および非インタラクティブモードで有効化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## エンタープライズゲートウェイの認証改善

エンタープライズゲートウェイでの認証情報の競合が防止され、ネイティブのオプショナルAPIキーサポートが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## gemini-3.1モデルのサポート

gemini-3.1モデルのエイリアスとthinking設定が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## 枯渇クォータモデルへのフォールバック

枯渇クォータモデルに対する安定したフォールバックルーティングが確保された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)

## バグ修正・改善

AUTO_EDITモードでのシェルリダイレクションが自動承認されるようになった。サブエージェントスレッドコンテキストが分離された。NixOSサンドボックスでのパーミッションエラーが解消された。ENAMETOOLONGおよびENOTDIRのファイルパース処理が修正された。PolicyEngineがACPセッションに統合されデッドロックが防止された。ripgrepのパス解決が1Passwordサポートとともに堅牢化された。ink worker-entry.jsおよびdevtoolsパッケージがバンドルされるようになった。macOSおよびWindowsでのpnpmグローバルインストールの自動検出が追加された。テーブルカラム幅のクランプが改善された。脆弱な依存関係が更新された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0)
