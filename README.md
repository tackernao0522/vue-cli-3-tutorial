# VueCLI

+ 参考: https://cli.vuejs.org/guide/installation.html <br>

## Vue Routerなし

+ `root $ docker compose run --rm vue create .`を実行<br>

+ `Manually select features` を選択して `enter`<br>

+ `Space`キーを押すと点いたり消えたりする<br>

+ 下記の状態で`Enter`<br>

```
Vue CLI v4.5.15
? Please pick a preset: Manually select features
? Check the features needed for your project:
❯◉ Choose Vue version
 ◉ Babel
 ◯ TypeScript
 ◯ Progressive Web App (PWA) Support
 ◯ Router
 ◯ Vuex
 ◯ CSS Pre-processors
 ◉ Linter / Formatter
 ◯ Unit Testing
 ◯ E2E Testing
```

+ `3.x`を選択して`Enter`<br>

+ `ESLint with error prevention only`を選択して`Enter`<br>

+ `Lint on save`を選択して`Enter`<br>

+ `In dedicated config files`を選択して`Enter`<br>

+ `Save this as a preset for futre projects? (y/N)` は `N`を入力して`Enter`<br>

+ `Use NPM`を選択して`Enter`<br>

+ `front/vue.config.js`を作成する<br>

```js:vue.config.js
module.exports = {
  devServer: {
    port: 8080,
    disableHostCheck: true,
  }
};
```

+ `$ npm install --save-dev html-webpack-plugin preload-webpack-plugin`を実行しておいた方が良い? (不明)<br>

+ 詳細: https://github.com/tackernao0522/udemy-aoki-vue/blob/main/README11.md <br>
　