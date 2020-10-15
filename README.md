# dev-beginner-tutorial

想定読者はプログラミング未経験だが、これからエンジニアとして研究・開発のアルバイトや仕事をスタートしようとしている人（理系学部生など）。最短で開発に参加するための基礎トレーニングするのを目標にする（50時間くらいを想定）。

## 目標

<details>
<summary>基本的なUnixコマンドが使える</summary>

- `ls`
- `cd`
- `cp`
- `mv`
- `grep`
- `curl`
- `ssh`
- ...
</details>

<details>
<summary>動的型付け言語（スクリプト言語）を一つ自由に使える</summary>

- **Python**: とくに科学技術計算の用途では現状これ一択
- Ruby: 日本製でWeb系で人気があるが正直やや下火
- Perl: 下火
- JavaScript: Web系の仕事をするなら必要
- **TypeScript**: Microsoft製の型付きJavaScript
- ...

</details>


<details>
<summary>静的型付け言語を一つ使える</summary>

- **C++:** 学習難易度が高いが最速
- Java: 求人が多い
- **C#:** Microsoft製Java
- Golang: Google製で文法が比較的シンプル
- **Rust**: C/C++代替を目指しており、モダンかつ安全性が高い
- ...
</details>


<details>
<summary>簡単な制御構文・データ構造・アルゴリズムを適切に使いこなしてプログラムが書ける</summary>

- for
- if
- 配列 (vector, list, ...)
- 連想配列 (map, dict, ...)
- 集合 (set)
- (Optional) 再帰関数
- (Optional) 深さ優先探索、幅優先探索
- ...
</details>

<details>
<summary>ソフトウェアのバージョン管理ができる (Git/GitHub)</summary>

- `git checkout`
- `git add`
- `git commit`
- `git push`
- `git fetch`
- `git merge`
- `git pull`
- ...
</details>

<details>
<summary>単体テストを書いて開発ができる</summary>

- 自分の使える言語で単体テストが書ける
- CIを設定できる
</details>

#### Optional

<details>
<summary>再現性のある環境で開発ができる (Docker)</summary>

- 用意されたDockerコンテナを利用できる
- Dockerfileを自前で用意できる
</details>

## トレーニングコース

 1. [Unixコマンド](./docs/01_unix_command.md)
 2. [Python文法](./docs/02_python.md)
 3. [Pythonにおける制御構文・データ構造の演習](./docs/03_python_quiz.md)
 4. [Gitをつかったソフトウェアのバージョン管理](./docs/04_git.md)
 5. [GitHubを使った開発](./docs/05_github.md)
 6. [Pythonにおける単体テストの書き方](./docs/06_python_unittest.md)
 7. [Python総合演習](./docs/07_python_practice.md)
     - Pythonを使ったパッケージ・CLIコマンド開発
     - Pythonで簡易ニューラルネットワーク開発
 8. [C++文法](./docs/08_cpp.md)
 9. [C++における制御構文・データ構造の演習](./docs/09_cpp_quiz.md)
10. [C++総合演習](./docs/10_cpp_practice.md)