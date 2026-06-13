## セッションタイトルの多言語対応

セッションタイトルが会話の言語で自動生成されるようになった。`language`設定で特定の言語を固定することも可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## footerLinksRegexes設定の追加

`footerLinksRegexes`設定が追加され、フッター行に正規表現にマッチしたリンクバッジを表示できるようになった。ユーザー設定またはマネージド設定で構成可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrockクレデンシャルキャッシュの改善

`awsCredentialExport`から取得したクレデンシャルが、固定の1時間ではなく`Expiration`まで正しくキャッシュされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## availableModelsの適用修正

エイリアスモデルの選択が`ANTHROPIC_DEFAULT_*_MODEL`環境変数を通じてブロックされたモデルにリダイレクトされなくなった。`/fast`は許可リスト外のモデルに切り替わる場合、トグルを拒否するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Fable 5のオートモード修正

Opus 4.8が有効でない組織でFable 5のオートモードが失敗する問題が修正された。分類器が利用可能な最良のOpusモデルにフォールバックするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フック条件のパスマッチング修正

Read/Edit/Writeツールのフック`if`条件で、`Edit(src/**)`、`Read(~/.ssh/**)`、`Read(.env)`などの文書化されたパターンが正しくマッチするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Linuxサンドボックスのシンボリックリンク修正

`.claude/settings.json`が絶対パスを対象とするシンボリックリンクの場合にLinuxサンドボックスが起動に失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## tmuxでのクリップボード修正

tmux over SSH環境で`/copy`およびマウス選択によるコピーがシステムクリップボードに反映されない問題が修正された。3.2より古いバージョンのtmuxペーストバッファの読み込みも修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Controlの修正

Web/モバイルからのRemote Control接続がセッションのモデルを無断で切り替える問題が修正された。切断通知が数値コードではなく人間が読める理由を表示するようになった。別のアカウントにサインインした際にセッションが正しく切断されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /cdおよびワークツリー移動の修正

`/cd`およびワークツリーの移動後にセッションが以前のディレクトリのgitブランチを表示し続ける問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsの修正

1つのウィンドウで戻るボタンを押しても、同じセッションに接続された他のウィンドウが切断されなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションの修正

`/bg`でターン中にバックグラウンドに移行した際、継続する処理がない場合に「Working」が永遠に表示される問題が修正された。PR URLによるエージェント検索で、スケジュールされたウェイクアップ中やジョブブロック中にオープンされたPRが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windows関連の修正

エージェントビューの入力でテキストカーソルが表示されない問題が修正された。`claude --bg -cn <name>`でセッション名が正しく設定されるようになった。バックグラウンドセッションがWindowsネットワークパスを永続化状態で無害化してからリスポーンするようになった。`~/.claude/daemon`にReadOnly属性が設定されている場合のバックグラウンドサービスデーモンの起動問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## その他の修正

破損した状態ファイルからの不正なレジュームIDによるバックグラウンドセッションのリスポーン拒否が修正された。自動更新をまたいで開いたままのウィンドウが返信を送信できない場合のガイダンスが改善され、`claude daemon status`でバージョンスキューの動作が説明されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)
