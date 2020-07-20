# daichi-design-portfolio
> Nuxt.js を使用したデザインポートフォリオ

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```
## Plugins
### vue-scrollto
ページ内リンクのスムーススクロールを簡単に実装できるプラグイン
npm：https://www.npmjs.com/package/vue-scrollto

#### 導入
```bash
npm install --save vue-scrollto
```

#### 設定
`/plugins/`に設定ファイルを作成する
本プロジェクトでは`/plugins/vue-scrollto.js/`で作成
アニメーションの`duration`等の設定をここで行う

`/nuxt.config.js`に記載されている`plugins`の箇所に、作成した`vue-scrollto.js`の
パスを指定することで、全ページでプラグインを使用することができる

#### 使用方法
`nuxt-link`で`vue-scroll-to`のプロパティを追加して、スクロールしたい`id`を指定
`nuxt-link`のプロパティで`to`が必須なので、指定せずにプロパティのみを設置する必要がある
`/components/Header.vue`等に使用例が記載

### vue-awesome-swiper.js
スライダーアニメーションを簡単に実装できるプラグイン
npm：https://www.npmjs.com/package/vue-awesome-swiper

#### 導入
```bash
npm install swiper vue-awesome-swiper --save
```

#### 設定
`/plugins/`に設定ファイルを作成する
本プロジェクトでは`/plugins/vue-awesome-swiper.js/`で作成
今回はこの`vue-awesome-swiper.js`ではアニメーション等の設定を行わず、定義のみを行っている

`vue-scrollto.js`と同様`/nuxt.config.js`に記載されている`plugins`の箇所に、
作成した`vue-awesome-swiper.js`のパスを指定することで、全ページでプラグインを使用することができる

#### 使用方法
今回は使用するコンポーネント、もしくはページ内の`data`で設定を行っている
`swiper`タグでスライダーの親BOXを作成し、`swiper-slide`タグでスライドの定義を行う
`/components/Section02.vue`等に詳細な設定や、使用方法の例が記載
