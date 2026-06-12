## マウスホイールスクロール加速の設定追加

`wheelScrollAccelerationEnabled`設定が追加され、フルスクリーンモードでのマウスホイールスクロール加速を無効化できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /modelピッカーのモデルファミリー表示修正

`/model`ピッカーがDefaultの解決先のモデルファミリーを非表示にしていた問題が修正された。Max/Team Premium/Enterpriseプランではopusが、Pro/Teamプランではsonnetが、従量課金APIアカウントではopusがそれぞれ独立した行として表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /modelピッカーのSonnetバージョンラベル修正

`ANTHROPIC_DEFAULT_SONNET_MODEL`で別のSonnetを指定している場合に、`/model`ピッカーがハードコードされたSonnetバージョンラベルを表示していた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Fable 5使用量クレジットバナーの修正

使用量ベースの課金を行うエンタープライズアカウントで「Fable 5 is now consuming usage credits」バナーが誤って表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrock GovCloudリージョンの推論プロファイル修正

Bedrock GovCloudリージョン（`us-gov-*`）で推論プロファイルのプレフィックスが`global`と誤って導出されていた問題が修正され、正しい`us-gov`プレフィックスが使用されるようになった。これにより派生モデルIDでの400エラーが解消された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションのプロバイダー環境変数継承修正

バックグラウンドセッションが、バックグラウンドデーモンを起動したシェルから別のセッションの`ANTHROPIC_*`プロバイダー環境変数（ゲートウェイURL、カスタムヘッダー、`/model`エイリアス）を継承していた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## シェルコマンド中断後の終了遅延修正

macOSおよびLinuxで、シェルコマンドが中断またはkillされた直後にClaude Codeを終了する際に発生していた1〜2秒の遅延が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## gitコミット共著者のモデル名修正

一部のモデルでgitコミットの共著者帰属に誤ったモデル名が表示されていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /advisorダイアログのモデル選択修正

`/advisor`ダイアログで、`availableModels`許可リストによってブロックされているアドバイザーモデルが事前選択されていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スキルホットリロードの効率化

スキルのホットリロードで、単一のスキルが変更された場合にスキル一覧全体を再送信していた問題が修正され、変更されたスキルのみが再通知されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Workflowツールのサブエージェント帰属ヘッダー修正

Workflowツールの`agent()`サブエージェントでエージェントごとの帰属ヘッダーが欠落していた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## VSCode使用量帰属ダイアログの追加

VSCodeのAccount & usageダイアログ（`/usage`）に使用量帰属が追加され、キャッシュミス、ロングコンテキスト、サブエージェント、スキル/エージェント/プラグイン/MCPごとの内訳が過去24時間または7日間で表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 事前ウォームバックグラウンドワーカーの認証修正

アイドル状態が続いた後にクレームされた事前ウォームバックグラウンドワーカーが「Could not resolve authentication method」エラーで失敗していた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)
