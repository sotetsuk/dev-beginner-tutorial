# dev-beginner-tutorial

想定読者はプログラミング未経験だが、これからエンジニアとして研究・開発のアルバイトや仕事をスタートしようとしている人（理系学部生など）。最短で開発に参加するための基礎トレーニングするのを目標にする（50時間くらいを想定）。

## :white_check_mark: 目標

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

- `git checkout (switch/restore)`
- `git add`
- `git commit`
- `git push`
- `git fetch`
- `git merge`
- `git pull`
- ...
</details>

<details>
<summary>単体テストを書いて開発を進めることが出来る</summary>

- 自分の使える言語で単体テストが書ける
- CIを設定できる
</details>

## :pencil: トレーニングコース

 1. [Unixコマンド](./docs/unix_command.md)
 2. [Python文法・演習](./docs/python.md)
 3. [Gitをつかったソフトウェアのバージョン管理](./docs/git.md)
 4. [GitHubを使った開発](./docs/github.md)
 6. [Python総合演習](./docs/python_practice.md)
     - Pythonを使ったパッケージ・CLIコマンド開発
     - Pythonで簡易ニューラルネットワーク開発
 7. [C++文法・演習](./docs/cpp.md)
 9. [Docker入門](./docs/docker.md)