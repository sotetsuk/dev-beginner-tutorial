# Gitをつかったソフトウェアのバージョン管理

ソフトウェア開発において、バージョン管理は必要不可欠です。
AppleStoreに行けば、すべてのアプリケーションはバージョンが明示されています。
バージョン管理をすることで、

1. 更新内容に説明を加える。
2. バージョン間の違いを簡単に比較する。　
3. 不具合が発生したときに前のバージョンに戻す。
4. 違うメンバー同士が同時にそれぞれ違う機能を開発して安全にマージする。

といったことが可能になります。
**Git**は現在もっとも多く使われているバージョンコントロールシステムです。
ここでは、Gitの使い方を学ぶことで、チームで協力して開発するための準備をします。

| <div style="text-align:center"><img src="/assets/version.png" width=400 /></div> | <div style="text-align:center"><img src="/assets/git.png" width=400 /></div> |
|:---:|:---:|
| AppleStoreにおけるアプリケーションのバージョン | Gitのソースコード自体もGitで管理されています github.com/git/git  |

## :desktop_computer: 事前準備（環境設定）

### Windows

- WSLのUbuntu上でgitがインストールされていることを確認してください `$ which git`
- もしなければ `$ sudo apt-get install git`

### Mac

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