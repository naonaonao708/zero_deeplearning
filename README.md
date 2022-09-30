# zero_deeplearning

![img](./zero_deeplearning_img.jpeg)


「ゼロから作るDeep LearningーーPythonで学ぶディープラーニングの理論と実装」の勉強ノート＆勉強日記


## Directory
```
.
├── README.md <-Logや情報をまとめる
├── info
│    └── deep-learning-from-scratch <-公式のGithub
├── oreilly-978-4-87311-758-4e.pdf <-「ゼロから作るDeep LearningーーPythonで学ぶディープラーニングの理論と実装」のPDF
└── wordbook.md <-分からない単語をまとめておく
```


## Data
-[ゼロから作る Deep Learning](https://github.com/oreilly-japan/deep-learning-from-scratch)
公式Github


## Log
### 20220730
昔買った「ゼロから作るDeep LearningーーPythonで学ぶディープラーニングの理論と実装」をちゃんと読むために、Githubで記録をつけながら機械学習の勉強をする<br>
リポジトリ作成<br>
1章Python入門、2章パーセプトロン終了<br>
1章はクラスのところだけなど一部だけやった

### 20220731
3章ニューラルネットワーク 3.4の３層ニューラルネットワークの実装まで終了<br>
ニューラルネットワークの所は難しく理解に時間がかかる<br>
oreilly-978-4-87311-758-4e.pdfを追加<br>
wordbookのMarkdownがズレてたので修正<br>

### 20220801
3章ニューラルネットワークの続きから<br>
3.6の実装はMNISTのデータを用いるため公式Githubのディレクトリで行った<br>
MINIST実装のpickleファイルの場所が不明<br>
4章ニューラルネットワークの学習4.2.2まで終了

### 20220802
4章ニューラルネットワーク4.2から<br>
4.2.3ミニバッチ学習、4.3数値微分をやった

### 20220803
4.4の勾配をやった<br>
4.3の数値微分の偏微分の復習も進めた

### 20220805
4.5学習アルゴリズムの実装　２層ニューラルネットワークのクラスの実装<br>
chap4のディレクトリにdatasetファイルをそのままコピペした→minist_loadを使うために<br>
本の表紙pngをディレクトリに置いた

### 20220806
4章ニューラルネットワークの学習終了<br>
この章は実装などが多く、内容も難しかったので時間がかかった<br>
4.5の二層ニューラルネットワークの実装の認識精度をグラフ化するところが分からなかった

### 20220808
5章誤差逆伝播に入った　ディレクトリも作成<br>
5.4単純なレイヤの実装まで終了　簡単な問題で乗算レイヤ・加算レイヤを実装した

### 20220809
funcディレクトリを作成→関数やレイヤをまとめて置いといてある<br>
func/layer.pyの途中　今までのクラスを追加しておきたい<br>
5.5 5.6まで終了→次は誤差逆伝播法の実装を

### 20220810
Vimのプラグインを入れた、最初はNomalモードでも日本語が挿入されるエラーが出てた→解決<br>
→参考[vscodeのvimでインサートモードからノーマルモードの戻るときに半角英数に自動で戻す](https://modest-mahavira-e86dcc.netlify.app/blog/vim-in-vscode-input-method/)<br>
前回の復習としてレイヤの関数を書いた<br>
5誤差逆伝播終了、またもう一周したり復習して内容を理解できるようにしたい

### 20220811
6章学習に関するテクニック初め<br>
6.1のパラメータの更新の途中まで、SGDの欠点について理解した

### 20220814
6.1パラメータ更新　Momentum・AdaGrad・Adamについて<br>
6.2重みの初期値について　XavierやHeなど初期値の大切さについて理解した<br>

### 20220815
6.3Batch Normalizationについて<br>

### 20220816
6.4正則化について学んだ、過学習を防ぐための方法としてWeight decay(荷重減衰)とDropoutがある。<br>
6.5ハイパーパラメータの検証では、ハイパーパラメータの性能を評価するために検証データを使うことを学んだ。

### 20220817
６章終了<br>
ハイパーパラメータの最適化について、ベイス最適化など　実装も

### 20220818
7章畳み込みニューラルネットワークを始めた　ディレクトリ、Notebook作成<br>
NotebookのMarkdown中に図を挿入するコマンドで本文のFigを埋め込むようにした<br>
```
<img src="~path~">
```
全結合層の問題点から畳み込み演算の必要性について学んだ。<br>
また畳み込み演算の問題点を解決するためにパディングを行う。

### 20220819
畳み込み演算のフィルターの位置の間隔をストライドという。<br>
3次元データの畳み込みの方法、またそのバッチ処理について<br>

### 20220821
CNNでのデータである4次元配列について、またそのデータの展開方法としてim2colを学んだ。<br>

### 20220822
Convolution(畳み込み)レイヤの実装について、今回はim2col関数を用いて畳み込みを行った。<br>

### 20220823
プーリング層について

### 20220825
プーリング層の実装

### 20220830
CNNの実装

### 20220922
久しぶりに再開　学会などで進められなかった<br>
CNN実装の続き→Reli,Affine,SoftmaxwithLossの関数が認識されてない→関数を呼び込む必要がある

### 20220925
CNN実装→Layerの関数はfunc/layer.pyにあった<br>
7.6 CNNの可視化, 7.7 代表的なCNNは軽く目を通した<br>
7章CNN終了<br>

### 20220926
8章ディープラーニング<br>
ディープラーニングの最近のトレンドや歴史について勉強した

### 20220930
８章ディープラーニングの未来について、これにてゼロから作るディープラーニング終了<br>
最後の方は少し駆け足になってたので、もう一度復習がてら読み返したい<br>