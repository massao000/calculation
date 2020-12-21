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
### 終了時にｎを選択した場合
![gif](https://user-images.githubusercontent.com/69783019/102720293-d5407b80-4336-11eb-9c3d-2926f58e8b72.gif)

「n」を選択した際「画面をクリア中」と出現し三秒後に上に書かれている結果が消えメニュー画面が表示される。

---

### 終了時にｙを選択した場合
![gif](https://user-images.githubusercontent.com/69783019/102720297-da9dc600-4336-11eb-8409-77994c8be920.gif)

「y」を選択した際「txtとcsvファイルが...」と表示されアプリと同じ階層に「record_file」ファイルが作成され結果がtxtとcsvファイルに書き込まれます。

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
モードの説明

1問目 5 x 3 = (入力待ち)
```
```
モードの選択：1
──────────────────────
モードの説明

1問目 5 x 3 = 20
正解(1秒後自動で次の問題)
```

```
モードの選択：1
──────────────────────
モードの説明

2問目 10 ÷ 7 = (入力待ち)
```
```
モードの選択：1
──────────────────────
モードの説明

2問目 10 ÷ 7 = 2
不正解 答え 1.42(1秒後自動で次の問題)
```
省略
```
モードの選択：1
──────────────────────
モードの説明

6問目 10 x 8 = (入力待ち)
```
最後に結果の表示
```
───────────┤結果表示├──
日付：2020-12-18 イージーモード
イージーモード
01: 5 x 3 = 20　正解
02: 10 x 8 = 2　不正解
>>>
06： 10 x 8 =　80 正解
問題数: 6
タイム: 00:30.13
正答率: 5/10 50%
──────────────────────
終了しますか？(y/n)：(入力待ち)
```
```
───────────┤結果表示├──
日付：2020-12-18 イージーモード
イージーモード
01: 5 x 3 = 20　正解
02: 10 x 8 = 2　不正解
>>>
06： 10 x 8 =　80 正解
問題数: 6
タイム: 00:30.13
正答率: 5/10 50%
──────────────────────
終了しますか？(y/n)：n
画面クリア中...(終わればスタートメニューが表示される)
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
モードの説明

1問目 36 ÷ 13 = (入力待ち)
```

```
モードの選択：2
──────────────────────
モードの説明

2問目 36 x 63 = (入力待ち)
```
省略
```
モードの選択：2
──────────────────────
モードの説明

問15, 62 + 43 = (入力待ち)
```
最後に結果の表示
```
───────────┤結果表示├──
日付：2020-12-18 ノーマルモード
01: 36 ÷ 13 = 2.76 正解
02: 36 x 63 = 2268 正解
>>>
15: 62 + 43 = 150 正解
問題数: 15
タイム: 00:30.13
正答率: 15/15 100%
──────────────────────
終了しますか？(y/n)：(入力待ち)
```
```
───────────┤結果表示├──
日付：2020-12-18 ノーマルモード
01: 36 ÷ 13 = 2.76 正解
02: 36 x 63 = 2268 正解
>>>
15: 62 + 43 = 150 正解
問題数: 15
タイム: 00:30.13
正答率: 15/15 100%
──────────────────────
終了しますか？(y/n)：n
画面クリア中...(終わればスタートメニューが表示される)
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
モードの説明

1問目 5 x 25 ÷ 3 = (入力待ち)
```

```
モードの選択：3
──────────────────────
モードの説明

2問目 57 x 234 + 1284 = (入力待ち)
```
省略
```
モードの選択：3
──────────────────────
モードの説明

30問目 57 ÷ 1284 = (入力待ち)
```
最後に結果の表示
```
───────────┤結果表示├──
日付：2020-12-18 ハードモード
01: 36 ÷ 13 = 2.769 正解
02: 36 x 63 = 2268 正解
>>>
30: 62 + 43 = 150 正解
問題数: 30
タイム: 05:52.13
正答率: 30/30 100%
──────────────────────
終了しますか？(y/n)：(入力待ち)
```
```
───────────┤結果表示├──
日付：2020-12-18 ハードモード
01: 36 ÷ 13 = 2.769 正解
02: 36 x 63 = 2268 正解
>>>
30: 62 + 43 = 150 正解
問題数: 30
タイム: 05:52.13
正答率: 30/30 100%
──────────────────────
終了しますか？(y/n)：n
画面クリア中...(終わればスタートメニューが表示される)
```
## 4:終了

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
    * Writing、Operator、Animatio、IntError、を定義ファイル
* `color.py`
    * Color、Escape、を定義ファイル
* 自動生成されるファイル
    * `data.csv`
        * 難易度、問題、タイム、正答率、が書かれる
    * `text.txt`
        * 日付、難易度、問題、問題数、タイム、正答率、が書かれる
* `calculation.exe`
    * これだけで起動できるようにする

## クラス一覧
* Writing
    * コマンドプロンプトに結果を表示させる
* Operator
    * ランダムで生成された数字で式を作る
* IntError
    * 例外処理
* Animation
    * 表示文字にアニメーションをつける
* Color
    * フォントカラー
* Escape
    * エスケープシーケンス
## クラス詳細
### Writing
* データ属性
    * Escape
        * 難易度
    * issue
        * 解答の問題
    * problem
        * 問題数
    * time_attack
        * タイム
    * correct_answer_rate 
        * 正答率
    * fraction
        * 解答できた問題数と問題数
* メソッド
    * show
        * 結果を表示
### Operator
* データ属性
    * からのリスト
        * 問題をまとめるリスト
    * からのリスト
        * csv用リスト
* メソッド
    * random_problem
        * ランダムに数字を作成
    * operation
        * ランダムに作成された問題の演算を決める
    * operation_hard
        * ランダムに作成された問題の演算を決める
    * end_time_show
        * スタートから終了までの解答のタイムを記録
    * text_file
        * テキストファイルに書き込む
    * csv_file
        * csv用のテキストを書き込む
    * division_operator
        * 割り算をする
    * multiplication_operator
        * 掛け算をする
    * subtraction_operator
        * 引き算をする
    * addition_operator
        * 足し算をする
    * division_operator_hard
        * ランダム演算子と割り算をする
    * multiplication_operator_hard
        * ランダム演算子と掛け算をする
    * subtraction_operator_hard
        * ランダム演算子と引き算をする
    * addition_operator_hard
        * ランダム演算子と足し算をする
    * answer_data
        * 演算の正解か不正解かを表示
### Animation
* メソッド
    * anim
        * 配列を順番に表示させる
    * start_loading
        * スタートのカウントダウン
    * end_loading
        * 終了のカウントダウン
### IntError
数値じゃない例外クラス

### Color
* フォントカラーの設定一覧
### Escape
* エスケープシーケンス（カーソル移動などを設定）

## モジュール
* os
* random
* time
* csv
* datetime
* colorama

## 備考
アプリケーションのある位置に新しくrecord_fileが生成され`data.csv`と`text.txt`が格納される
|記入内容|`text.txt`|`data.csv`|
|:---:|:---:|:---:|
| 日付 | ○ | ✕ |
|難易度| ○ | ○ |
| 問題 | ○ | ○ |
| 問題数 | ○ | ✕ |
| タイム | ○ | ○ |
| 正答率 | ○ | ○ |

`data.csv`と`text.txt`にどんどん追記されていきます。
