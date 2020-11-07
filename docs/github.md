# GitHub入門

## :ok: これだけ！GitHub上での開発の流れ

はじめに、ここで学ぶことの結論をまとめてしまいます。GitHub上では、**Issueベースでのタスク管理**と、**Pull Request (PR) ベースでの開発**を行います。
    
[![issue](assets/issue.png)](https://github.com/sotetsuk/dev-beginner-tutorial/issues)

!!! important "Issueベースでのタスク管理"

    何か必要な機能や修正があれば、まずIssueを作成して「なぜこの機能・修正が必要なのか」「その仕様は何なのか」を書き出します。
    実際に開発に移る機能や修正は、Issueリストの中から優先順位やタスクの依存関係などに応じて決定します。


!!! important "Pull Request (PR) ベースでの開発"

    1. 実装する機能・修正の仕様を決めます（解決するIssueを決めます）。
    1. `main` に移り、リモートリポジトリから最新の変更を取り込みます。 `git switch main && git pull origin main`
    2. 新しい機能を実装するブランチを `main` から作ります。 `git switch -c <branch name>`
    3. ブランチ上で機能を実装します。
        3. 変更を実装し、適宜コミットします。 `git add <file>` `git commit -m "<commit message>"`
        4. 適宜プッシュします。 `git push -u origin <branch name>` 特に、最初のコミット直後には一度プッシュしてPRを作り、Issueと関連付けます。
    5. 機能が完成したら、レビュー前に最新の `origin/main` を取り込みます。 `git fetch && git merge --no-ff origin/main` （競合が発生した場合は解決する）
    6. レビューを経てPRを `main` に "Squash And Merge" でマージします。

## :question: なぜGitHubの使い方を学ぶのか？

GitHubは、最も広く使われているソフトウェア開発のプラットフォームです。
前章で学んだGitのリポジトリを管理してくれる他、開発に必要な様々な便利な機能を提供してくれています。
多くのソフトウェアがGitHub上でオープンソースソフトウェア（OSS) として開発されており、
開発者がGitHub上で開発されたソフトウェアを使わない日はありません。
大学でも会社でも、チームでの開発においてGitHubを使う可能性はかなり高く、Gitに加えてGitHubの使い方を習得するのは現代エンジニアにとって必須だと言えます。

## :orange_book: GitHubを用いた基本的な開発の流れ

> [GitHub Flow (Japanese translation)](https://gist.github.com/Gab-km/3705015)

## :police_officer: Git/GitHubでの開発におけるルール

## :book: TIPS

絶対というわけではないが、よく見かけるある程度合理的なTIPSです。

!!! tip "Mergeを "Squash And Merge" にする"

!!! tip "ブランチ名に作業者の名前や変更の種類を先頭につける"

    誰がどんな変更を加えているブランチなのかの視認性が少し良くなります。

    - `sotetsuk/feat/new-nn-model`
    - `sotetsuk/refactor/remove-comments`
    - `sotetsuk/docs/how-to-use`

## :dizzy: オススメの設定

設定ファイル `~/.gitconfig` を次のように編集してみましょう。

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

!!! quote ""
    - [gitのpush.defaultに関するノウハウ | Qiita](https://qiita.com/awakia/items/6aaea1ffecba725be601)
    - [git merge 時は必ずマージコミットを作るようにする | Hatena blog](https://neos21.hatenablog.com/entry/2017/06/18/080000)

## :pencil: 演習

このドキュメント自体もGitHub上で書かれています :fontawesome-brands-github: 

!!! important ""

    [github.com/sotetsuk/dev-beginner-tutorial](https://github.com/sotetsuk/dev-beginner-tutorial)

:white_check_mark: このドキュメントのリポジトリに、実際にPRを作成して送ってみましょう。
[index.md](https://github.com/sotetsuk/dev-beginner-tutorial/blob/main/docs/index.md)の足跡に自分のGitHubのアイコンを追加してみましょう。

:white_check_mark: また、このチュートリアル自体のコンテンツについても修正点を考えてIssueやPRを送ってみましょう。
例えば、次のようなPRを送ってみて下さい。

!!! example ""

    1. タイポをIssueで報告する and/or PRで修正する。
    2. 表記ゆれをIssueで報告する and/or PRで修正する。
    3. 不正確・誤っている説明をIssueで報告する and/or PRで修正する。
    4. 要望・改善案をIssueで報告する。

