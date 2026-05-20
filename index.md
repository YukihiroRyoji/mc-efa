# 概要
探索的因子分析のモンテカルロシミュレーションを簡便に行うためのRの関数を作成しています。
* R packageの形式になっています

## packageのダウンロード
[ダウンロード](simefa_0.0.1.0.tar.gz)

## インストール
```r
install.packages("パス/simefa_0.0.1.0.tar.gz", repos = NULL, type = "source")
```
psych packageを内部で使っていますので，入っていない場合はpsych packageもインストールしておいてください。

## 削除
不要になった場合，以下でRの環境から削除することができます。
```r
remove.packages("simefa")
```