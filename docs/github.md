# GitHub入門

!!! important "これだけ覚える！GitHub上での開発の流れ"

    基本的には次の1.~6.を繰り返すだけです。

    1. `main` にチェックアウトし、リモートリポジトリから最新の変更を取り込む。 `git switch main && git pull origin main`
    2. 新しい機能を実装するブランチを `main` から作る。 `git switch -c <branch name>`
    3. ブランチ上で機能を実装していく。
        3. 変更を実装し、適宜コミットする。 `git add <file>` `git commit -m "<commit message>"`
        4. 適宜 `git push -u origin <branch name>` する。特に、最初のコミット直後には一度プッシュしてPRを作る。
    5. 機能が完成したら、レビュー前に最新の `origin/main` を取り込む。 `git fetch && git merge --no-ff origin/main` （競合が発生した場合は解決する）
    6. レビューを経てPRを `main` にマージする。


## :question: なぜGitHubの使い方を学ぶのか？

## :orange_book: GitHubを用いた基本的な開発の流れ


> [GitHub Flow (Japanese translation)](https://gist.github.com/Gab-km/3705015)

## :police_officer: Git/GitHubでの開発におけるルール

## :book: Git/GitHubにおける慣習

絶対というわけではないが、よく見かけ、合理性のある者たち。

参加しているプロジェクトの慣習に合わせるのが良いと思われます。

### Mergeは"Squash And Merge"にする

### ブランチ名に作業者の名前や変更の種類を先頭につける。

!!! example ""

    - sotetsuk/feat/new-nn-model
    - sotetsuk/refactor/remove-comments
    - sotetsuk/docs/how-to-use

## :dizzy: オススメの設定

`~/.gitconfig` 

```yaml
[user]
        name = <YOUR NAME>
        email = <YOUR E-MAIL>
[alias]
        sw = switch
        br = branch
[push]
        default = current
[merge]
    ff = false
[pull]
    ff = only
```

> - [gitのpush.defaultに関するノウハウ | Qiita](https://qiita.com/awakia/items/6aaea1ffecba725be601)

## :pencil: 演習

このドキュメント自体もGitHub上で書かれています。
PRを作成して送ってみましょう。