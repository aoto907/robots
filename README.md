# ver2, ver3d
- レイノルズ・ボイドモデル（整列・結合・反発）＋ 回避行動 ＋ 抵抗力を用いて途中まで作成した群れの様子
- 捕食者はローレンツアトラクターに従った軌道を描き，被食者の群れを襲う．被食者はその行動に対して回避する

## 環境
### 言語
- python: jupyter で動かしています
### ライブラリ
- numpy: 計算を高速化（アップロードしたファイルには，あまり用いていない）
- matplotlib.pyplot: 描画用
- matplotlib.animation: 描画アニメーション（pyplot + animation により動画がを作る）
- cipy.integrates.solve_ivp: 捕食者の軌道（ローレンツアトラクター）の微分を計算するため

# png, image.py
- ５つのパターンで筆記した文字の分類器
- cnnで学習し分類します

## 環境
### 言語
- python: ubuntuで動かしていますが，vscodeでも動くと思います。
### ライブラリ
- keras: 機械学習フレームワーク
  - utils.np_utils: 正解ラベル付け
  - models.Sequential: モデルを用意（その後，各層の機構を定義する。引数や引用）
  - layers.convolutional.Conv2, MaxPooling2D: 画像サイズ，畳み込み
  - layers.core.Dense, Dropout, Activation, Flatten: 各層，情報削減(過学習の防止)，活性化関数，データの結合
- numpy: 計算の高速化
- sklearn.model_selection.train_test_split: 学習用と検証用へ分割するために
- PIL.Image: 画像の読み込みや編集など
- glob: ファイル操作
