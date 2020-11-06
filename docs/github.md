# GitHub入門

!!! important "これだけ！GitHub上での開発の流れ"

    !!! note "Issueベースでのタスク管理"

        何か必要な機能や、修正必要なバグがあれば、まずIssueを作成します。


    !!! note "PRベースでの開発"

        1. 優先順位に基づいて、実装する機能・修正の仕様を決める（解決するIssueを決める）。
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
> - [git merge 時は必ずマージコミットを作るようにする | Hatena blog](https://neos21.hatenablog.com/entry/2017/06/18/080000)

## :pencil: 演習

このドキュメント自体もGitHub上で書かれています。

PRを作成して送ってみましょう。
例えば、次のようなPRを送ってみて下さい。

1. タイポを修正する。
2. 表記ゆれを修正する。
3. 不正確・誤っている説明を修正する。

もし何も変更する点が思いつかなければ、[README.md]()