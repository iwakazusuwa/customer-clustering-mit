# customer-clustering-mit

[![Python](https://img.shields.io/badge/Python-3.10+-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

階層的クラスタリング（Ward法）を用いて顧客データをグループ分けする Python スクリプトです。  
デンドログラムによる可視化とクラスタ数の指定で、顧客セグメンテーションを行います。

---

## 対象者

- 顧客データを階層的クラスタリングで分析したい方
- デンドログラムを用いてクラスタ構造を可視化したい方
- Python スクリプトを用いて簡単に分析を実行したい方

---

## 概要

このプロジェクトは、顧客データに対して Ward 法による階層的クラスタリングを適用し、  
デンドログラムを描画してクラスタ構造を可視化します。  
また、指定したクラスタ数での分割結果を CSV ファイルとして出力します。

---

## 特徴

- Ward 法による階層的クラスタリングの実装
- デンドログラムの描画と閾値によるクラスタ分割
- クラスタ数指定による分割も対応
- 出力結果を CSV 形式で保存
- Windows/Mac/Linux で出力フォルダを自動オープン

---

## インストール

```bash
git clone https://github.com/iwakazusuwa/customer-clustering-mit.git
cd customer-clustering-mit
pip install pandas numpy scipy matplotlib
```


# 使い方
このスクリプトは、コマンドライン操作なしで、ファイルをダブルクリックするだけで実行できます。



1. 2_data/sample.csv に分析したい顧客データを準備してください。
2. 1_flow/clustering.py を実行します。
```
python 1_flow/clustering.py
```
3. 結果は 3_output/ フォルダに以下のファイルとして保存されます：
 - dendrogram.png：デンドログラム画像
 - clusters.csv：クラスタ番号付きの顧客データ


# ファイル構成
```
├── 1_flow/
│   └── clustering.py         # クラスタリング処理スクリプト
├── 2_data/
│   └── sample.csv            # 入力データ（顧客情報）
├── 3_output/
│   └──                      # 結果の保存フォルダ（自動生成）
```

# 注意事項
 - 入力データのカラム名や形式が異なる場合、スクリプト内の設定を変更してください。
 - クラスタ数の指定はデンドログラムを参考に適切に設定してください。

# 今後の展望
 - 他のクラスタリング手法（例：K-means, DBSCAN）との比較機能の追加
 - 入力データの前処理機能の強化
 - 可視化機能の拡充（例：3D プロット、インタラクティブな可視化）

# 貢献方法
プロジェクトへの貢献は以下の方法で歓迎します：
 - バグ報告や機能追加の提案は Issues で
 - コード改善や新機能追加は Pull Request で
 - ドキュメント改善や翻訳も歓迎


# LICENSE
MIT License（詳細はLICENSEファイルをご参照ください）

### 開発者： iwakazusuwa(Swatchp)


