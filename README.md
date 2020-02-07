NICT日本語辞書
====

概要
----

[CRFSegmenter](https://github.com/hiroshi-manabe/CRFSegmenter)で使われる日本語の辞書です。

以下のようにファイルが分かれています。

- nictdict.tsv 一般辞書（普通名詞・用言・機能語などを含む）
- nictdict_ne.tsv 固有名詞辞書
- nictdict_declinable.tsv 用言辞書

形式
----

辞書の形式はUTF-8エンコードのタブ区切りテキストです。

辞書のフィールド数は6で、各フィールドは左から以下の順になっています。

- 読み
- 発音
- 品詞
- 活用タイプ（非用言の場合は"*"）
- 表記
- 代表形（「表記-読み」形式；後述）

