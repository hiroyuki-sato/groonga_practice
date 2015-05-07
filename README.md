
## Groonga 学習用スクリプト

[Groonga](http://groonga.org/)の[チュートリアル](http://groonga.org/ja/docs/tutorial.html)にあるサンプルテーブルを作成するためのスクリプトです。

## 構成

```
.
|-- README.md
|-- bin
|   |-- clean        # データベース削除スクリプト
|   |-- gen_chap4_1  # 4.1. 基本的な操作
|   |-- gen_chap4_3  # 4.3. いろいろなデータの保存
|   |-- gen_chap4_4  # 4.4. さまざまな検索条件
|   |-- gen_chap4_5  # 4.5. ドリルダウン
|   |-- gen_chap4_6  # 4.6. タグ検索・参照関係の逆引き
|   |-- gen_chap4_7  # 4.7. match_columnsパラメータ
|   |-- gen_chap4_8  # 4.8. パトリシア木による前方一致検索
|   |-- gen_chap4_10 # 4.10. マイクロブログ検索システムの作成
|   `-- gen_chap4_10 # 4.11. クエリ拡張
|-- databases # データベース出力ディレクトリ
`-- etc
    `-- functions #
```

## 利用方法

例えば「4.1. 基本的な操作」のデータを作成したい場合は次のようにコマンドを実行します。

```
cd bin
./gen_chap4_1
```

`databases`ディレクトリに`chap4_1.db`を作成します。

次のコマンドで4.1にあるselect分などを試してください。

```
groonga chap4_1.db
```

## 削除

`clean`コマンドでdatabasesディレクトリのchap4*を削除します。

```
cd bin
./clean
```
