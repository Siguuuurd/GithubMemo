# Promise(executor)
http://mithril-ja.js.org/promise.html


### Promise(約束・契約・保証．．．言葉の意味と機能がまったく一致してないような気が・・・)
下記のURLから文章を抜粋した。
http://azu.github.io/promises-book/#chapter1-what-is-promise
- Promiseは非同期処理を抽象化したオブジェクトとそれを操作する仕組み。

- Promiseでは、このような非同期に対するオブジェクトとルールを仕様化して、 
統一的なインターフェース(オブジェクト指向言語のインターフェースと似たような意味)で書くようになっており、
それ以外の書き方は出来ないようになっている。

- Promiseという統一されたインターフェースがあることで、 そのインターフェースにおけるさまざまな非同期処理のパターンを形成することができる。
つまり、複雑な非同期処理等を上手くパターン化できるというのがPromiseの役割であり、 Promiseを使う理由の一つである。

#### Promise Overview
ES6 Promisesの仕様で定義されているAPIは大きく分けて以下の3種類ある。
[参考(わかりやすい)][http://azu.github.io/promises-book/#chapter1-what-is-promise]

+ ** Constructor **
Promiseは XMLHttpRequest のように、コンストラクタ関数である Promise からインスタンスとなる promiseオブジェクトを作成して利用する。
promiseオブジェクトを作成するには、Promise コンストラクタを new でインスタンス化する。

+ ** Instance Method **
newによって生成されたpromiseオブジェクトにはpromiseの値を resolve(成功) / reject(失敗) した時に呼ばれる コールバック関数を登録するために
promise.then() というインスタンスメソッドがある。

Promise というグローバルオブジェクトには幾つかの静的なメソッドが存在する。
Promise.all() や Promise.resolve() などが該当し、Promiseを扱う上での補助メソッドが中心となっている。



** ※※※Promiseについては量が多いため、これ以上は割愛する。[http://azu.github.io/promises-book/#chapter1-what-is-promise]が分かりやすいので参考にする。