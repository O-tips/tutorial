# hugo-bookの記法

詳しくは [hugo book公式](https://themes.gohugo.io/themes/hugo-book/)を参照

こちらに[Example site](https://hugo-book-demo.netlify.app/docs/shortcodes/tabs/)もあります．
- Shortcodesの欄などが参考になるかも
- ソースが見たい場合は[GitHub](https://github.com/alex-shpak/hugo-book/tree/main/exampleSite)から

## ディレクトリ
- 各ディレクトリに`_index.md`というファイルを作成する。
- 各ファイルの最初にメタデータを書け、これにより左のバーの階層が変わる
- 詳しくは[Page Configuration](https://themes.gohugo.io/themes/hugo-book/#page-configuration)を参照

## その他機能
// TODO



## 書いてる時のメモ
- \#\#で右側に色々出るから基本\#は２個からがいいかも
- 画像の入れ方
  - [こちら](https://qiita.com/atuyosi/items/4100bd502e373c088c74)を参考
  - [公式ドキュメント](https://gohugo.io/content-management/shortcodes/#figure)に詳しく載ってる
  - e.g. `{{< figure src="/images/image.jpg" title="title" width="320" height="320">}}`