NICT日本語辞書
====

概要
----

[CRFSegmenter](https://github.com/hiroshi-manabe/CRFSegmenter)で使われる日本語の辞書です。

以下のようにファイルが分かれています。

- nictdict.tsv 一般辞書（普通名詞・用言・機能語などを含む）
- nictdict_ne.tsv 固有名詞辞書
- nictdict_declinable.tsv 用言辞書

ライセンス
----------

[LICENSE.md](/LICENSE.md)をご参照ください。


形式
----

辞書の形式はUTF-8エンコードのタブ区切りテキストです。

辞書のフィールド数は6で、各フィールドは左から以下の順になっています。

- 読み
- 発音
- 品詞
- 活用タイプ（非用言の場合は"*"）
- 表記
- 代表形（「表記-読み」形式）

### 読み

単語の読みを片仮名で記述します。「学校」であれば「ガッコウ」のような、一般的なかな書き表記です。

### 発音

単語の発音を片仮名で記述します。具体的には、「読み」と以下のような場合に違うものになります。

- 長音（学校：ガッコー）
- ヂ、ヅ（鼻血：ハナジ）
- 助詞の「は」「へ」「を」、またそれに由来するもの（それでは：ソレデワ）

### 品詞

IPADICの品詞体系をベースにしています。

pos_table_ipadic.tsv をご参照ください。

### 活用タイプ

IPADICの活用型をベースにしています。

pos_table_ipadic.tsv をご参照ください。

### 活用について

[活用について](/inflection.md)をご参照ください。

### 表記

単語の実際の表記を記述します。

### 代表形

その単語を代表する表記と読みのペアを記述します。

この欄をキーとして使うことにより、表記ゆれ等をまとめることができます。

例としては、以下のようなものがあります。

    ウィンドウ	ウィンドー	名詞-一般	*	ウィンドウ	ウィンドウ-ウィンドウ
    ウィンドゥ	ウィンドー	名詞-一般	*	ウィンドゥ	ウィンドウ-ウィンドウ
    ウィンドー	ウィンドー	名詞-一般	*	ウィンドー	ウィンドウ-ウィンドウ
    ウインドウ	ウインドー	名詞-一般	*	ウインドウ	ウィンドウ-ウィンドウ
    ウインドー	ウインドー	名詞-一般	*	ウインドー	ウィンドウ-ウィンドウ

    ヒナマツリ	ヒナマツリ	名詞-一般	*	ひな祭り	ひな祭り-ヒナマツリ
    ヒナマツリ	ヒナマツリ	名詞-一般	*	雛まつり	ひな祭り-ヒナマツリ
    ヒナマツリ	ヒナマツリ	名詞-一般	*	雛祭	ひな祭り-ヒナマツリ
    ヒナマツリ	ヒナマツリ	名詞-一般	*	雛祭り	ひな祭り-ヒナマツリ
    ヒナマツリ	ヒナマツリ	名詞-一般	*	ひなまつり	ひな祭り-ヒナマツリ
