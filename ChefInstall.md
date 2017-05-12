# Chefのインストールと設定

参考サイト：[http://note.miyabis.jp/2013/12/chef-%E3%82%92-windows-%E3%81%A7%E4%BD%BF%E3%81%A3%E3%81%A6%E3%81%BF%E3%82%8B.html]

# Chefのインストール
1. Chef Client をダウンロード。

[URL]: http://www.opscode.com/chef/install/#options
または
[URL]: http://opscode.com/chef/install.msi

コマンドプロンプトで下記を実行するとバージョンが表示される。
chef-solo -v


1. Windows 環境用の Cookbook 取得
以下の２つを取得する。
http://community.opscode.com/cookbooks/windows
http://community.opscode.com/cookbooks/chef_handler


1. chef-solo の設定
C:?chef?solo.rb

```以下を入力する
cookbook_path ["C:?chef?repo?cookbooks"]
```

1. chefで圧縮ファイルを解凍とかするときにコマンドで実行できる解凍ツール(7-zip)[Inx-7-zip]
[Inx-7-zip]: https://supermarket.chef.io/cookbooks/seven_zip "chefで圧縮ファイルを解凍とかするときにコマンドで実行できる解凍ツール(7-zip)"

```以下を入力する
C:?chef?repo フォルダに下記の内容で 7-zip.json ファイルを作成する。
{
	"run_list": ["recipe[7-zip]"]
}
```
