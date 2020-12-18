# 企画

## アプリケーション概要

計算力を鍛えるアプリケーションです。
# 機能一覧

* 1:イージーモード
* 2:ノーマルモード
* 3:ハードモード
* 4:終了

### モードの説明
| モード | 問題数 |出る数字|演算子数|
|:---:|---:|:---|:---:|
|イージーモード|3~6|1~10|1個|
|ノーマルモード|5~15|1~100|1個|
|ハードモード|10~30|10~10000|1~2個|
|終了|
# 動作イメージ

## デモ
gifを入れる

## 起動メッセージ

```calculation.exe
──────────┤メニュー├───
1:イージーモード (3~6 問) 
2:ノーマルモード (5~15 問)
3:ハードモード (30 問)
4:終了
──────────────────────
モードの選択：(入力待ち)
```

## 1:イージーモード
```
モードの選択：1
──────────────────────
モードの説明
エンターを押すとスタート
```
この時の表示は上書きされ新しく問題が表示される
```
モードの選択：1
──────────────────────
問1, 5 x 3 = (入力待ち)
```
```
モードの選択：1
──────────────────────
問1, 5 x 3 = 20
正解(1秒後自動で次の問題)
```

```
モードの選択：1
──────────────────────
問2, 10 ÷ 7 = (入力待ち)
```
```
モードの選択：1
──────────────────────
問2, 10 ÷ 7 = 2
不正解(1秒後自動で次の問題)
```
省略
```
モードの選択：1
──────────────────────
問6, 10 x 8 = (入力待ち)
```
最後に結果の表示
```
モードの選択：1
──────────────────────
───────────┤結果表示├──
イージーモード
問題
問1, 5 x 3 = 20　正解
問2, 10 x 8　不正解
>>>
問6, 10 x 8 =　80 正解
問題数: 6
タイム: 00:00.00
正答率: 5/10 50%
──────────────────────
```

## 2:ノーマルモード

```
モードの選択：2
──────────────────────
モードの説明
エンターを押すとスタート
```
この時の表示は上書きされ新しく問題が表示される
```
モードの選択：2
──────────────────────
問1, 36 ÷ 13 = (入力待ち)
```

```
モードの選択：2
──────────────────────
問2, 36 x 63 = (入力待ち)
```
省略
```
モードの選択：2
──────────────────────
問15, 62 + 43 = (入力待ち)
```
最後に結果の表示
```
モードの選択：2
──────────────────────
───────────┤結果表示├──
ノーマルモード
問題
問1, 36 ÷ 13 = 2.769 正解
問2, 36 x 63 = 2268 正解
>>>
問15, 62 + 43 = 150 正解
問題数: 15
タイム: 00:00.00
正答率: 15/15 100%
──────────────────────
```
## 3:ハードモード

ハードモードでは演算子が3つになることがある

```
モードの選択：3
──────────────────────
モードの説明
エンターを押すとスタート
```
この時の表示は上書きされ新しく問題が表示される
```
モードの選択：3
──────────────────────
問1, 5 x 25 ÷ 3 = (入力待ち)
```

```
モードの選択：3
──────────────────────
問2, 57 x 234 + 1284 = (入力待ち)
```
省略
```
モードの選択：3
──────────────────────
問30, 57 ÷ 1284 = (入力待ち)
```
最後に結果の表示
```
モードの選択：2
──────────────────────
───────────┤結果表示├──
ハードモード
問題
問1, 36 ÷ 13 = 2.769 正解
問2, 36 x 63 = 2268 正解
>>>
問30, 62 + 43 = 150 正解
問題数: 30
タイム: 00:00.00
正答率: 30/30 100%
──────────────────────
```

## 4:終了

```
モードの選択：4
──────────────────────
モードの説明
エンターを押すとスタート
```

```
モードの選択：4
──────────────────────
終了します: 5(カウントダウンの表示)
```
カウントダウンですぐに終了しないようにする
---

# 設計
## ファイル
* `calculation.py`
    * メインプログラム
* `operator.py`
    * OperatorClassを定義ファイル
    
* どっちかにするか両方か
    * `data.csv`
        * 結果などをまとめる
    * `text.txt`
        * 結果などをまとめる
* `calculation.exe`
    * これだけで起動できるようにする

## 実装予定クラス一覧
* OperatorClass
    * 演算子をつけるクラス(問題を作る)
* EndTimeClass
    * 問題開始時から終了までの時間の計測
* WritingClass
    * 結果などをまとめるクラス
* intError
    * 数値ではない物の例外処理
## クラス詳細
### Operator
* データ属性
    * number_first
        * ランダムの数値
    * number_second
        * ランダムの数値
    * number_third
        * ランダムの数値
### EndTime
* 未定
    * 未定
        * 未定
### Writing
* 未定
    * 未定
        * 未定
### intError
数値じゃない例外クラス

## モジュール
* time
* os
* random

## 備考
calculation.exeで新たに作成された`data.csv`or`text.txt`に以下を記入していく
* モード
* 実行した日付
* 問題
* 問題数
* スタートから終わるまでのタイム
* 正答率

できれば演算子は問題ごとにランダムに変わる

43 ÷ 56 = 0.7678571428 みたいな出た場合小数点第2(0.76)まで入力
