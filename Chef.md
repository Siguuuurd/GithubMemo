# Chef
***
以下のURLの内容の覚書き。かなりわかりやすい。

http://qiita.com/kasaharu/items/55a3000db31c52ce0bd7

***

## 概要
***
- ミドルウェアの設定やアプリケーションのインストールなどのサーバ構築を自動化するためのツールで、今はやりの Infastructure as Code
- サーバの増強などに合わせたインフラの構築の自動化やデプロイ時の環境整備にも有用
- 従来の手順書がそのままコードになるため、メンテナンスもしやすい 
	- バージョン管理やテストができる
- 複数の同一環境を構築することに向いているため、Vagrant などと組み合わせることでプロジェクトメンバー間で開発環境を統一することにも利用できる


## Chef の構成
***
- Chef には大きく "Chef-Server/Client 構成" と "Chef-Solo 構成" がある
- 規模にもよるが、個人的には "Chef-Solo 構成" で十分なイメージ (そして Chef-Solo しか使ったことありません)

### Chef-Server/Client 構成
***
* Chef-Server, Node, Workstation の 3 コンポーネントから成る

#### Chef-Server
+ Node 情報の管理
+ Cookbook の管理
+ Client の認証

#### Node
+ 管理対象サーバで Chef-Client が動く
+ Chef-Server に問い合わせ、Cookbook を適用

#### Workstation
+ Cookbook の開発はここで行う
+ Cookbook を Chef-Server にアップロード

### Chef-Solo 構成
***
- Server も Client も必要としないスタンドアローン版
- 対象のマシンにコマンドとして Chef を適用する


## 簡単な用語説明
***
### Recipe (レシピ)
- Resource の定義(サーバの設定)が書かれるファイル
- 従来の手順書にあたるもの
- Ruby で記述でき、次のようなファイルに成る 
	-  これは、git-core というパッケージを apt なり yum なりでインストールするということを示す
	-  正確には、対象のサーバに対し "git-core が入った状態であること" という状態を記載している
	-  OS の差分は Chef が吸収するため、基本的には考えなくて良い(例外はある)
```default.rb
package "git-core" do
  action :install
end
```
### cookbook (クックブック)
- Recipe を含め、その他必要なファイルやデータがまとまったディレクトリ
  
### kitchen (キッチン)
- 単にリポジトリとも呼ばれる
- Chef の実行に必要な関連ファイル群
