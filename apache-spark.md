# Pythonで入門するApache Spark

Speaker: Tatsuya Atsumi

spark2.0をベースに説明

## 特徴

* 分散処理で面倒な障害発生時の復旧作業などはspark側でうまくしてくれる
* インメモリによる処理

## Core API

### RDD

* クラスタ上に分散したデータを束ねるオブジェクト
* Sparkでプログラミングする際はRDDだけを意識すれば良い
* ファイル読み込みの命令を行なっても，実際には読み込まれず本当に使うタイミングで読み込むようになっている
  * 障害時の復旧のためらしい

## Spark SQL

### Dataframe

* SQLライクにかける
* コードを減らすことができる(RDDに比べて)
* RDDに比べて細かい調整が不要
  * Spark側で最適化するのでどの言語で書いても処理時間が大して変わらない

## MLlib

* ``spark.ml`` を使う
* パイプラインAPI
  * In/OutはDataframe
  * Estimator
    * 学習処理を行うプロセス
