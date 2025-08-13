# customer-clustering-mit
階層的クラスタリングを用いて顧客をグループ分けするPythonスクリプトです。
顧客データを読み込み、クラスタリング結果を可視化・保存します。

# 特徴
- Ward法による階層的クラスタリングの実装
- デンドログラムの描画と閾値によるクラスタ分割
- クラスタ数指定による分割も対応
- 出力結果をCSV形式で保存
- Windows/Mac/Linuxで出力フォルダを自動オープン

# 必要環境
Python3系が必要です。  

必要なパッケージは以下のコマンドでインストールしてください。

```
pip install pandas numpy scipy matplotlib
```

# 使い方
このスクリプトは、コマンドライン操作なしで、ファイルをダブルクリックするだけで実行できます。

1. 2_data/sample.csv に分析したい顧客データを用意してください。
1. 1_flow/clustering.py を実行します。
1. 3_output フォルダに結果の画像とCSVファイルが保存されます。


# 注意点
ファイル名や場所を変えたい場合は、スクリプト内の設定を変更してください。


# ファイル構成
```
├── 1_flow/
│   └── clustering.py         # クラスタリング処理スクリプト
├── 2_data/
│   └── sample.csv            # 入力データ（顧客情報）
├── 3_output/
│   └──                      # 結果の保存フォルダ（自動生成）
```

## LICENSE
MIT License（詳細はLICENSEファイルをご参照ください）

### 開発者： iwakazusuwa(Swatchp)
