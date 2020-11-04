# Gitをつかったソフトウェアのバージョン管理

App Storeに行くと、アプリケーションのバージョンが明示されています。何故でしょうか？

ソフトウェア開発において、バージョン管理は必要不可欠です。
残念ながら多くのヒトは（本人が思っているほど）賢くありません。
例えば、プログラムを書いていると、次のようなことが頻繁に起こります。

- 一時間前には動いていたソースコードが、何故か今は動かないし、**この一時間の間で加えた変更の一体どこが原因かも分からない。**
- 半年前に自分の書いた奇妙な修正があるが、**一体何故そんな修正をしたのか全く分からない。**

上の２つのような悲劇的な自体が一人で開発していても起こりうるわけですから、チームで開発すると事態はより一層悲壮感を増します。
こうした喜劇のような悲劇を防ぐために、バージョン管理が有効です。
バージョン管理を適切に行うと、次のようなことが可能になります。

1. 変更・更新内容に説明を加える。
2. バージョン間の違いを簡単に比較する。　
3. 不具合が発生したときに前のバージョンに戻す。
4. 違うメンバー同士がそれぞれ違う機能を同時に開発して、マージする。

そして、**Git**は現在最も多く使われているバージョンコントロールシステムです。
2020年現在、プログラミング言語の選択肢は数多くあれど、バージョンコントロールシステムの選択肢はGitだけと言って過言ではありません。
ここでは、Gitの使い方を学ぶことで、チームで協力して開発するための準備をします。

### 身近なバージョン管理の例
App Storeでは、アプリケーションのバージョンと、その更新内容が記述されています。

<div style="text-align:center"><img src="/assets/version.png" width=600 /></div>


### "GitのGitリポジトリ"

[github.com/git/git](https://github.com/git/git)

奇妙なようで当然のことですが、Gitのソースコード自体もGitを使って管理されていおり、2020年現在も更新され続けています。

<div style="text-align:center"><img src="/assets/git.png" width=600 /></div>

## :desktop_computer: 事前準備（環境設定）

### Windows

- WSLのUbuntu上で `git` がインストールされていることを確認してください: `$ which git`
- もしなければ `$ sudo apt-get install git`

### Mac

- ターミナルから `git` がインストールされていることを確認して下さい: `$ which git`
- もしなければ [Homebrew](https://brew.sh/) を使って `$ brew install git`

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