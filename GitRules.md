### ブランチ命名規則
- Issueと同じ名前にする（Issueは "feat/components/Hearder" のようにする予定）

### バグがあった場合
- fix: ... のようにIssueを立てる（bugラベルをつける）
- fixの場合、無理にIssueとBranch名を合わせなくて大丈夫

### PR作成
- こちらの「プルリクエストに必要な情報を入れよう」参考に
  - [チーム開発におけるプルリクの作法](https://qiita.com/ikuwow/items/fb52a54c086398eb5b92)
- 併せて、冒頭に "Issue: #3" のように書いてください（IssueとPRを紐づけるため）

### PR確認
- Reviewerにはご自身以外の2名を選択してください
- なるべく2名でレビューしたいですが、状況により1名だけでもMergeします

----------------

リモートの最新版を取得する
```
git pull origin develop（ブランチ名）--rebase
```

ブランチを切ってそのブランチに移動
```
git switch -c ブランチ名
```
