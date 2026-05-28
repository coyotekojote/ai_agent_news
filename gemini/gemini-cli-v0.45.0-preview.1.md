## PTYリサイズ時のクラッシュ防止

v0.45.0-preview.0に対するパッチリリース。PTYリサイズ操作がネイティブクラッシュに対して強化され、リサイズ前にプロセスの生存確認を行うことでレースコンディションによるクラッシュが防止されるようになった。EBADFエラーの検出範囲も拡張された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.45.0-preview.1)
