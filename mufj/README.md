# 三菱UFJが出してるコンペ

https://signate.jp/competitions/754

## 自然言語が混ざった教師ありの2値分類タスク

<P>初めてのタスク</p>

### 方針
1. preprocessing
	1. カテゴリ変数の数値化(goalをohe,他をle)
	2. html_contentをトークン化 
		1. html_contentの中身をgoogle transにかける(??→ja→en)
	3. 
2. アンサンブルのやり方？
	1. KFoldで分割した塊毎にモデルを分ける?
  2．ほかのモデル(Robertaなど)で回すことを試みる
  

4. GBDTらへんを試したい
	何も考えずに突っ込んでみても良いかも？
  one-hot encodingの必要はないが、label encodingの必要はあり。
  テキストの数値化(ベクトル化)も必要。


---

### 写経してみて

- 勉強になった
  1. テキスト列の要素をひとまとめにして新しいカラムを作るアイデア
  2. driveにInputフォルダ、Outputフォルダを作成しておく事
  3. KFoldの作法。

