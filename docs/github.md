# GitHub入門

## :question: なぜGitHubの使い方を学ぶのか？

## :orange_book: GitHubを用いた基本的な開発の流れ

!!! important ""
    1. `master/main` にチェックアウトし、リモートリポジトリから最新の変更を取り込む `git switch main && git pull origin main`
    2. 新しい機能を実装するブランチを `master/main` から作る `git switch -c <branch name>`
    3. 変更を実装し、コミットする `git add <file>` `git commit -m "<commit message>"`
    4. `git push`
    5. Ask review
    6. Squash small changes if needed
    7. Merge

> [GitHub Flow (Japanese translation)](https://gist.github.com/Gab-km/3705015)

## :police_officer: Git/GitHubでの開発におけるルール

## Git/GitHubにおける慣習

絶対というわけではないが、よく見かけ、合理性のある者たち。

参加しているプロジェクトの慣習に合わせるのが良いと思われます。

### MergeはSquash and Mergeにする

### ブランチ名に作業者の名前や変更の種類を先頭につける。

!!! example ""

    - sotetsuk/feat/new-nn-model
    - sotetsuk/refactor/remove-comments
    - sotetsuk/docs/how-to-use


## オススメの設定

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
```

> [gitのpush.defaultに関するノウハウ](https://qiita.com/awakia/items/6aaea1ffecba725be601)

## :pencil: 演習

このドキュメント自体もGitHub上で書かれています。
PRを作成して送ってみましょう。