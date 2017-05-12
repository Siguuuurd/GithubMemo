# Githubいろいろ


## ファイルを戻す方法
ファイルを戻すたり、取り消したりする方法は
多くある。今知っているのはごく一部。

1. Commitを取り消す場合
Source Treeで「Commitの打ち消し」する。
ファイルがいらない場合はファイルの破棄、または削除をする。
破棄と削除の違いは？


1. Pushしたファイルを戻したい場合
もう一度Pushする。これが定番らしい。
もしPushしたファイルが多く、Pull RequestをClosedして
新しいPull Requestしてもよい場合は、「Create Pull Request」後に
「Closed Pull Request」をすれば、MergeされずPushしたファイルが削除される。
他の方法はないか？


1. Mergeしてしまったファイルを取り消す場合
Revertする。
Masterのファイルを直接上書きしてしまった場合の対処方法は？ 
他にはないか？



## trelloとGithub連携
なんか連携できるとか？



## Githubの常識？
### Issueについて
1. Issueを立てた人はAssainに設定しなくてもコメントのメールが送られてくる。
1. Assainに設定されて人はコメントのメールが届く。
1. Assainに設定されていない場合、mention(@teinoue)をコメントにつけるとメールが送られる。

### PullRequestはファイル削除でClosedしてはいけない。
そんなことしたら猛省せよ。
ファイルを更新し直したり、過去のファイルに戻すべき、とのこと。


### CommitのタイトルにIssueの番号を忘れずに

### [WIP]をつけて開発中とわかるようにすること
Create Pull Requestタイトルの先頭につける。
例)
[WIP]WIPつけようＺＥ☆彡！

### タグ付けしようＺＥ☆！
ＺＥ☆！ってなんだよ。
・・・ググったらカオスでした。
死んでも言わない。

## Github、Gitlab自分のPCでサーバ建てられる
便利なので使おう。



