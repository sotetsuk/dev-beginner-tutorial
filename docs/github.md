# GitHub入門

## :question: なぜGitHubの使い方を学ぶのか？

## :orange_book: GitHubを用いた基本的な開発の流れ

!!! important ""
    - `master/main` にチェックアウトし、リモートリポジトリから最新の変更を取り込む `git switch main && git `
    - Checkout to your new feature branch
    - Implement changes (follow one purpose and keep it small)
    - Test your changes (e.g., make sure it passes build)
    - Ask review
    - Squash small changes if needed
    - Merge

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