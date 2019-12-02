# sassを勉強する
## setup
1. vscode拡張プラグインのインストール
    - Browser Preview
    - Live Sass Compiler
    - Live Server

1. Live Server設定
    - Use browser Previewにチェックを入れる

## 使い方
- index.htmlとindex.scssを用意する
- 下の青いバーのWatch Sassをクリック
- index.sassと同じディレクトリにindex.cssが生成される
    - watching中はsassが更新されるとcssも自動更新される
- index.htmlで右クリック Open with live serverをクリック
- ブラウザウィンドウが展開され、表示される。自動更新。

## note

### 変数
- 変数は$で定義できる
[サンプル](./fields/scss/index.scss)

### ネストして定義することができる
[サンプル](./nest/scss/index.scss)

### Mixins（関数）
- @mixinで関数を定義することができる
[サンプル](./mixins/scss/index.scss)

### animation
[サンプル](./sandbox/scss/index.scss)

### アニメーションのブラウザサポート

##### ブラウザサポートによって、接頭辞が必要

- デフォルト
    - ```keyframes```
    - ```transition```
    - ```transform-translate```

- Firefox 4 
    - ```@-moz-keyframes```
    - ```-moz-transition-property:width```
    - ```-moz-transform-translate:1s```

- Safari and Chrome
    - ```@-webkit-keyframes```
    - ```-webkit-transition-property:width```
    - ```-webkit-transform-translate:1s```

- Opera
    - ```@-o-keyframes```
    - ```-o-transition-property:width```
    - ```-o-transform-translate:1s```

### 参考リンク
- [keyframes（CSS3）とSassでイケてるアニメーションをシンプルなコードで実装する方法](http://liginc.co.jp/web/html-css/css/105796)
- [SCSS アニメーションを簡単に実装するmixinとか](https://chaika.hatenablog.com/entry/2015/03/08/144120)
- [要素を順番にフワッと表示するアニメーションを CSS の animation プロパティで作る](https://memocarilog.info/webdesign/8050)
- [【UIデザイナー必見】動きが面白い！目を引くこと間違いなしのCSSアニメーション集part1](https://webdesignfacts.net/entry/css-animation-part1/)
- [WordPressで美容室のサイトを流行りのCSSアニメーションを使って作った](https://arutega.jp/block_reveal_effects/)
- [【CSS3】@keyframes と animation 関連のまとめ](https://qiita.com/7968/items/1d999354e00db53bcbd8)