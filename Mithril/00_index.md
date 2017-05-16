#Index

![画像1](https://github.com/Siguuuurd/GithubMemo/blob/master/image/usagi2.png "画像")


## Mithrilとは？

### Mithrilのサイト
http://mithril-ja.js.org/
Mithrilはシングルページアプリケーションを構築するためのモダンなクライアントサイドのJavaScriptフレームワークです。
サイズは小さく（< 8kb gzip）高速で、ラウティングやXHRといったユーティリティもパッケージ内に内蔵しています。


### CodeZineサイト
https://codezine.jp/article/detail/8815
Mithrilは、VirtualDOMを採用したデータバインディング型JavaScriptフレームワークです。
軽量、高速をコンセプトに作られているため、モバイル向けのシングルページアプリケーションに最適なフレームワークと言えます。


#### VirtualDOMとは 
データバインディング型フレームワークで生じる、DOMの更新を最小限にとどめるための仕組みです。
JSオブジェクトなどを使い仮想的にDOMのツリー構造を作成し、変更差分を算出する仕様のため、高度なDOMの処理を自前で行わなくても、
最適化された差分計算の仕組みによりDOMが更新されます。細かい実装方法はフレームワークによって異なりますが、


レンダリングパフォーマンスが向上するメリットがあります。日本ではVirtualDOM Advent Calendar 2014がキッカケとなり、
「VirtualDOM」対応のJavaScript Frameworkが一般的にも注目され始めてきました。
代表的なフレームワークはReact、mercury、Elmです。2015年5月現在ではReactが人気です。



### 参考サイト
#### Mithrilのサイト
http://mithril-ja.js.org/
#### モバイル向けシングルページアプリに最適！ 軽量JSフレームワーク【Mithril】 - 基礎編
http://codezine.jp/article/detail/8815?p=2
