# Memo

### チーム開発でよく使用する主なコマンド一覧

|                                         | 用途                 |
|-----------------------|-----------------------|
|git clone {url}                          |	リモートからローカルにコピー    | 
|git add .	                              |  共有するファイルを選択する     |
|git commit 	                            |  変更したファイルをGitに登録    |
|git push	                                |  local repository→ remote repository |
|git switch	                              | ブランチ切り替え            |
|git switch -c	                          | ブランチ作成&切り替え        |
|git branch　                              | 今いるブランチを確認する      |
|git pull origin ブランチ名 --rebase	        | ブランチを最新の状態にする    | 

`--rebase`ってしているのは `git pull` をしたときに不要なコミットを防ぐためです。

git pull origin ブランチ名 --rebaseしたあとにnode_modulesがないとエラーを吐きます。
```
npm install
```
でnode_modulesを作成できます（はじめてgit cloneしたときは含まれていないので必ず必要）

### その他のリンク

- [コミットメッセージの書き方について](https://qiita.com/konatsu_p/items/dfe199ebe3a7d2010b3e)
- [プルリクエストの作成方法
](https://docs.github.com/ja/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- [Pull Request レビューをリクエストする
](https://docs.github.com/ja/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review)
- [チーム開発におけるプルリクの作法](https://qiita.com/ikuwow/items/fb52a54c086398eb5b92)
- [質問の仕方](https://qiita.com/seki_uk/items/4001423b3cd3db0dada7)
