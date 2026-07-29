## 自動更新通知の改善

自動ダウンロードされた更新に対して`/restart`の提案が表示されるようになり、警告スタイリングが控えめになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-3)

## 大規模マルチファイルdiffのレンダリング改善

`/diff`コマンドで大規模なマルチファイルdiffがスクロールとシンタックスハイライト付きで高速に処理されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-3)

## 分割ビューサイドバーの改善

ホバーでフォーカスする機能がデフォルトで無効になった（`sidebar.hoverFocus`で設定可能）。アクティブセッションカードのアクセントがデフォルトで有効になった（`sidebar.accentActiveSession`で設定可能）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-3)

## web_fetchのリダイレクト対応

`web_fetch`がHTTPリダイレクトに追従するようになった。クロスオリジンリダイレクトの場合はパーミッションが要求され、リダイレクト元が表示される。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-3)

## 未送信プロンプトのセッション保持

セッション切り替え時に未送信のメッセージテキストが元のセッションに保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-3)

## セッション再開時のモード維持

セッション再開時にオートパイロットまたはプランモードが維持されるようになり、インタラクティブモードに戻らなくなった。`task_complete`などのモード固有ツールも保持される。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-3)

## URLパーミッションプロンプトの修正

URLパーミッションプロンプトで、ホスト統合がプロンプトを再生成した際にサンドボックスバイパス警告とモデルの推論が保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-3)
