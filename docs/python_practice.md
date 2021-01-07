# Python総合演習
ここでは、今でに学習したUNIXコマンド、Python、Git/GitHubを活用した実際の開発の演習を行います。

## :orange_book:  Pythonを使ったパッケージ・CLIコマンド開発

こちらの教材の内容を再構築して、Python開発の手順を学びましょう。
この教材では、今までに学んだ内容も復習しながら、単体テストや型ヒントを用いた開発についても説明しています。

[github.com/sotetsuk/python-dev-tutorial](https://github.com/sotetsuk/python-dev-tutorial)


## :pencil: 演習 

:white_check_mark: これまで学習してきたUNIXコマンド/Python/Git/GitHub/単体テストの知識を活かしつつ、自分の身近な問題や興味なる事柄を解決するPythonパッケージまたはCLIコマンドをGitHub上で開発してみましょう。

**題材例**

1. [Tic-Tac-Toe](https://ja.wikipedia.org/wiki/%E4%B8%89%E7%9B%AE%E4%B8%A6%E3%81%B9)のPythonパッケージ
2. [ポモドーロ・テクニック](https://ja.wikipedia.org/wiki/%E3%83%9D%E3%83%A2%E3%83%89%E3%83%BC%E3%83%AD%E3%83%BB%E3%83%86%E3%82%AF%E3%83%8B%E3%83%83%E3%82%AF)のCLIツール


## :orange_book:  Pythonで簡易ニューラルネットワーク開発
人工知能技術の発展は目覚ましく、ニューラルネットワークの仕組みを理解することも、エンジニアにとってある種の必修科目となりつつあります。簡略化されたニューラルネットワークライブラリを自作してみて、その中身を知りましょう。

## :pencil: 演習 

[github.com/joelgrus/joelnet](https://github.com/joelgrus/joelnet)のリポジトリ内容をビデオを見ながら自分で再構築して、簡易ニューラルネットワークライブラリを作ってみましょう。

## :pencil: 追加演習 (optional)

:white_check_mark: 自分で再構築した簡易ニューラルネットワークライブラリで、手書き文字認識の分類をやってみよう。 ([Recognizing hand-written digits](https://scikit-learn.org/stable/auto_examples/classification/plot_digits_classification.html))

:white_check_mark: LossとAccuracyの学習途中の変遷を[Tensorboard](https://www.tensorflow.org/tensorboard?hl=ja)を使って可視化してみよう。ここではTensorflowやPyTorchのようなTensorboard対応のフレームワークを使うわけではないので、[tensorboardX](https://github.com/lanpa/tensorboardX)を利用してみましょう。

:white_check_mark: 手書き文字認識の分類性能が高くなるハイパーパラメータを自分でいくつか試して探してみましょう。このとき、[過学習](https://www.tensorflow.org/tutorials/keras/overfit_and_underfit?hl=ja)に注意しよう。
