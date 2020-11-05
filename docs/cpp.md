# C++入門

## :question: なぜC++を学ぶのか

ここで学ぶ**C++**は[静的型付け言語](https://ja.wikipedia.org/wiki/%E9%9D%99%E7%9A%84%E5%9E%8B%E4%BB%98%E3%81%91)の一つになります。
C++に限らず、静的型付け言語を学ぶメリットは数多くあります。
静的型付け言語は、プログラムの実行より前のコンパイル時に変数の型が決定されます。
実行より前に型の整合性チェックが入ることで、コンパイルエラーによって型に関するバグを事前に検知することができます。
これは特に、大型のソフトウェアをチームで開発するときに役に立ちます。
また、[統合開発環境](https://ja.wikipedia.org/wiki/%E7%B5%B1%E5%90%88%E9%96%8B%E7%99%BA%E7%92%B0%E5%A2%83)がプログラムを解析しやすくなり、よりリッチな入力補完が効きます。
そして、一般に静的型付け言語の実行速度は、Pythonのような動的型付け言語の実行速度よりも数倍から数十倍以上高速です。

C++特有の長所も存在します。C++は全ての静的型付け言語を含めても、実行速度が[最速](https://benchmarksgame-team.pages.debian.net/benchmarksgame/which-programs-are-fastest.html)な言語だと考えられています。
低レイヤのプログラミングも可能なこともあり、より高速で効率的な演算が求められるアプリケーションの開発において重宝されています。

!!! example "C++を使っているプロジェクト例"
    - [Tensorflow](https://github.com/tensorflow/tensorflow) Google製ニューラルネットワークフレームワーク
    - [PyTorch](https://github.com/pytorch/pytorch) Facebook製ニューラルネットワークフレームワーク
    - [ONNX Runtime](https://github.com/microsoft/onnxruntime) Microsoft製ニューラルネットワーク推論ライブラリ
    - [OpenCV](https://github.com/opencv/opencv) 画像認識ライブラリ

!!! note "Pythonと科学技術計算"

    Pythonは人工知能を始めとして多くの科学技術計算分野で幅広く活用されています。
    実行速度が遅いのになぜこうした分野で広く活用されているのか疑問に思う方もいるかもしれませんが、それはPythonの科学技術計算ライブラリが、実際には内部がC言語などの他の言語で書かれていたり、[BLAS](https://ja.wikipedia.org/wiki/Basic_Linear_Algebra_Subprograms)や[LAPACK](https://ja.wikipedia.org/wiki/LAPACK)のような線形代数演算ライブラリを呼び出したりして高速化されているためです。
    実際、Pythonの代表的な科学技術計算ライブラリである[NumPy](https://ja.wikipedia.org/wiki/NumPy)は、その33%がC言語で書かれています。
    
    > [https://github.com/numpy/numpy](https://github.com/numpy/numpy)


## :computer: 事前準備（環境設定）

[CLion](https://www.jetbrains.com/ja-jp/clion/)を使って開発します。

## :orange_book: C++文法の学習

[C++入門 AtCoder Programming Guide for beginners (APG4b) | AtCoder](https://atcoder.jp/contests/APG4b)

## :pencil: 演習

Pythonで一度解いた、[AtCoder Beginners Selection | AtCoder](https://atcoder.jp/contests/abs/tasks) の問題をC++で解き直してみましょう。

## :gift: 付録

[江添亮のC++入門](https://ezoeryou.github.io/cpp-intro/) 