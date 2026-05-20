# 概要
探索的因子分析のモンテカルロシミュレーションを簡便に行うためのRの関数を作成しています。
* R packageの形式になっています

# packageのインストール／削除
## ダウンロード
[ダウンロードファイル](simefa_0.0.1.0.tar.gz)
* ファイル名は simefa_0.0.x.y.tar.gz のようになっています。x, yはバージョンによって異なります。

## インストール
```r
install.packages("ダウンロードしたファイル名", repos = NULL, type = "source")
```
* RStudioを使っている場合，メニューからインストールすることも可能です。
- Tools -> Install Packages ... -> Install From: で Package Archive File (zip; tar.gz)を選ぶ -> ファイルを選択
* psych packageを内部で使っていますので，入っていない場合はpsych packageもインストールしておいてください。

## 削除
不要になった場合，以下でRの環境から削除することができます。
```r
remove.packages("simefa")
```

# 関数

# 使用例

