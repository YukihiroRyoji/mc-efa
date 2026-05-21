([Home](https://yukihiroryoji.github.io))

# 概要
探索的因子分析のモンテカルロシミュレーションを簡便に行うためのRの関数を作成しています。
* R packageの形式になっています
## 更新履歴
* 2026/5/20 最初のリリース(0.0.1)

# packageのインストール／削除
## ダウンロード
[ダウンロードファイル](simefa_0.0.1.tar.gz)
* ファイル名は simefa_x.y.z.tar.gz のようになっています。x, y, zはバージョンによって異なります。

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

# 使用例
* [シミュレーション例1](simefaex1.html)
* [シミュレーション例2](simefaex2.html)
* （以下，作成中）

# 関数
各関数のhelpはRの中で表示できます（現在のところ日本語で記述）

## 因子モデルの表示等
* factor_model ：因子負荷行列と因子間相関行列から，因子モデルを出力
* set_factor_model_from_dataset ：実データセットに因子分析を行い，母集団モデルとして使うパラメータを作る

## シミュレーションデータの生成
* gen_efa_data ：因子モデル，サンプルサイズ，シミュレーション回数を指定して，データを生成する
* gen_efa_data_categorical ：段階評定データを生成する
* gen_multiple_efa_data ：サンプルサイズを複数条件設定して，データを生成する
* sampling_from_dataset ：実データセットから指定の条件でサンプリングしてシミュレーションデータを作る

## 生成したデータに対して因子分析を実行し結果を要約
* run_efa_sim ：gen_efa_dataやgen_efa_data_categoricalで生成したデータを分析して要約
* run_multiple_efa_sim ：gen_multiple_efa_dataで生成したデータを分析して要約

## 因子数決定のシミュレーション
* sim_n_of_factors.parallel ：平行分析で因子数決定のシミュレーションを行う

# summary, plot関数
* run_multiple_efa_sim の出力には，summary関数とplot関数があります（シミュレーション例2も参照）

## その他
* congruence_coef
* get_efa_data
* fit_efa_sim

([Home](https://yukihiroryoji.github.io/))
