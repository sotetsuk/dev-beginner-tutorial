# ディープラーニング
人工知能技術の発展は目覚ましく、ニューラルネットワークの仕組みを理解することも、エンジニアにとってある種の必修科目となりつつあります。

## :orange_book: 学習教材

- [ゼロから作るDeep Learning ― Pythonで学ぶディープラーニングの理論と実装](https://www.oreilly.co.jp/books/9784873117584/)の第一章 (1.5, 1.6) と第二章〜第五章を読んで、ディープラーニングの基本を勉強してみて下さい。

## :pencil: 演習（Pythonで簡易ニューラルネットワーク開発）

[github.com/joelgrus/joelnet](https://github.com/joelgrus/joelnet)のリポジトリ内容をビデオを見ながら自分で再構築して、簡易ニューラルネットワークライブラリを作ってみましょう。

## :pencil: 追加演習 (optional)

:white_check_mark: 自分で再構築した簡易ニューラルネットワークライブラリで、手書き文字認識の分類をやってみよう。 ([Recognizing hand-written digits](https://scikit-learn.org/stable/auto_examples/classification/plot_digits_classification.html))

:white_check_mark: LossとAccuracyの学習途中の変遷を[Tensorboard](https://www.tensorflow.org/tensorboard?hl=ja)を使って可視化してみよう。ここではTensorflowやPyTorchのようなTensorboard対応のフレームワークを使うわけではないので、[tensorboardX](https://github.com/lanpa/tensorboardX)を利用してみましょう。

:white_check_mark: 手書き文字認識の分類性能が高くなるハイパーパラメータを自分でいくつか試して探してみましょう。このとき、[過学習](https://www.tensorflow.org/tutorials/keras/overfit_and_underfit?hl=ja)に注意しよう。
