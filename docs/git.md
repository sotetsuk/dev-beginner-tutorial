# Gitをつかったソフトウェアのバージョン管理

## :desktop_computer: 事前準備（環境設定）

### Windows

- WSLのUbuntu上でgitがインストールされていることを確認してください `$ which git`
- もしなければ `$ sudo apt-get install git`

#### Mac

- ターミナルからgitがインストールされていることを確認して下さい `$ which git`
- もしなければ[Homebrew](https://brew.sh/)を使って `$ brew install git`

## :blue_book: 学習教材

[git入門 | ドットインストール](https://dotinstall.com/lessons/basic_git)

## :white_check_mark: 習熟度チェック

:heavy_check_mark: これらのコマンドが何をするコマンドか分かるか確認しましょう。見覚えがない場合、どんなコマンドか調べてみましょう。

- `git status`
- `git add`
- `git push`
- `git commit`
- `git checkout`
- `git checkout -b`
- `git pull`
- `git fetch`
- `git clone`
- `git grep`
- `git diff`
- `git log`
- `git rm`
- `git merge`
- `git reset`
- `git revert`
- `git rebase`

:heavy_check_mark: 新しいバージョンのgitでは、`git checkout`の代わりに`git switch/restore`を使うことが推奨されています。`git checkout`のコマンドと`git switch/restore`の対応について調べてみましょう。

- `git checkout <branch name>` = ???
- `git checkout -b <new branch name>` = ???
- `git checkout -- <file name>` = ???