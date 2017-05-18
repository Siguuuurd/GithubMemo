# m（セレクタ、属性、子）
MithrilビューのHTML要素を表します。

[参考URL][https://mithril.js.org/hyperscript.html]

このm()関数は実際にはDOM要素を返しません。
代わりに、仮想DOMノード、または生成されるDOM要素を表すjavascriptオブジェクトであるvnodeを返します。

** ※HTMLに表示したい場合は、「m.render」を使用する。 **


## 仮想DOMノード(vnode)
- ** Mithrilサイト **
以下のURLは仮想DOMノードについて記載している。少しだけvnodeも記載されている。
レンダリング：ウェブブラウザがHTMLなどからウェブページを表示する。
http://mithril-ja.js.org/vnodes.html

- ** Qiitaサイト **
タイトル「なぜ仮想DOMという概念が俺達の魂を震えさせるのか」
http://qiita.com/mizchi/items/4d25bc26def1719d52e6

- ** teratail **
ざっくりした内容。QAのサイト
https://teratail.com/questions/41054

- ** 仮想DOMの内部の動き(VDOMあるいはVNode) **
http://postd.cc/the-inner-workings-of-virtual-dom/
濃い、長い、すべて読んでない

## 仮想DOMノードを調べた結果
よくわからなかった。
なんとなくふわっと記憶残ったのは以下通り。

- JavaScriptでHTML書く。
- 従来のPostなどしていたときとは違って画面はかわらない。
これをシングルページアプリケーションというらしい。

- スピードはjQueryよりかなり早いらしい。
- JavaScriptのMVC, MVW(Whatever)フレームワークのViewに位置あたるらしい。
- 「jQueryのDOM操作で汚れきったフロントエンドを救う救世主。」と謳うサイトもある。
確かにjQueryは作りこんでいくうちに複雑になりやすく、結果本人しかわからないぐらいボリュームと複雑になる。
そういうjQueryのプログラムは解析に時間がかかる。目が痛くなるし混乱するし、できれば避けたい。
そういうのを解消してくれるのが仮想DOMノードという救世主、とふわふわした感じで理解した。
Mithrilを解析などしてくうちに具体的なものがわかるかもしれないし、ついていけいかもしれない。
