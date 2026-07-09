## 使用量制限リセットクレジットの改善

使用量制限のリセットクレジットにタイプと有効期限が表示されるようになり、どのクレジットを使用するか選択できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## `writes`アプリ承認モードの追加

宣言された読み取り専用アクションを許可しつつ、書き込み操作にはプロンプトを表示する`writes`アプリ承認モードが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## MCPツールのインタラクティブ認証

MCPツールが実験的オプトインなしでインタラクティブに認証をリクエストできるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## アプリサーバーホストによるランタイム認証提供

アプリサーバーホストがランタイム時にCodexの認証を提供し、ログイン成功後にホストされたページにリダイレクトできるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## グローバルpnpmインストールの検出

グローバルpnpmインストールが検出されるようになり、診断やアップデートで正しいパッケージマネージャーが使用されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## Ultraリーズニング選択時の警告

Ultraリーズニングを選択した際に、高いマルチエージェント並行性が使用量を急速に増加させる可能性があることを警告するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## ChatGPTスレッドの廃止モデル復旧

再開されたChatGPTスレッドでコンパクションが廃止されたモデルを参照している場合、現在選択されているモデルでリトライすることで復旧するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## Intel macOSでのCode Modeクラッシュ修正

Intel macOSのリリースバイナリでCode Modeがクラッシュする問題が修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## Windowsサンドボックスのファイル操作改善

Windowsサンドボックスセッションで書き込み可能なルート内のファイル削除と、管理されたプライマリランタイムへのアクセスが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## ペーストされたターミナル制御シーケンスの無害化

ペーストされたターミナル制御シーケンスがTUIレンダリングや再開された会話履歴を破壊しなくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## アプリセッションの認証自動リフレッシュ

長時間実行されるアプリセッションで、ホストされた`codex_apps`コネクタの期限切れ認証が自動的にリフレッシュされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## Responses WebSocketの低遅延トランスポート維持

Responses WebSocketがシステムプロキシやカスタム認証局を尊重しつつ、低遅延トランスポートを引き続き使用するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## デバイスコードログインのフィッシング警告

デバイスコードログインの警告で、フィッシング試行の認識と停止方法が説明されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## プラグインスキル読み込みの高速化

リモートエグゼキューターでの名前空間解決をルートごとに1回に統合することで、プラグインスキルの読み込み時間が短縮された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## `/review`ブランチピッカーの改善

大規模リポジトリでの`/review`ブランチピッカーの速度と信頼性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## 自動レビューの動作改善

自動レビューの動作がより明確な指示とフォーカスされたツールセットで改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)

## Amazon BedrockモデルのGPT-5.6ファミリー明示化

Amazon Bedrockのモデル名がGPT-5.6ファミリーとバリアントを明確に識別するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.144.0)
