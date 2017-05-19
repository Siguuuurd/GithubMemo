#Hyperscript

デフォルトでは、Mithrilのビューはhyperscriptを使って定義されています。
Hyperscriptは、複雑なタグのHTMLよりも自然に字下げできる簡潔な構文を提供します。
また、その構文は単純にJavascriptなので、Javascriptツールのエコシステムを多く活用することができます。
例えばBabel、JSX（インラインHTML構文拡張 ）、eslint（linting）、uglifyjs（minification）、
istanbul（コードカバレッジ）、flow（静的型分析）など。
 Hyperscriptを使うと、複雑なタグを持つHTMLよりも自然にインデントできる、完結な構文でテンプレートが記述できます。
それに加えて、Babel, JSX (インラインのHTML文法拡張), eslint (構文チェック), uglifyjs (コードサイズ縮小化),
istanbul (コードカバレッジ), flow (静的な型解析) などのさまざまなJavaScriptのツールを活用することができます。
m(selector, attributes, children)