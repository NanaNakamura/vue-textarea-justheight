# vue-textarea-justheight

テキストエリア内で、  
入力文字数によって高さが変更されるコンポーネント  
※ リサイズにも対応

💫<a href="https://nananakamura.github.io/c/vue-textarea-justheight/index.html" target="_blank">Demo</a>


## Usage

### HTML
```
<template>
  <TextareaJustHeight v-model="data"/>
</template>
```

### scripts

.vueファイルコンポーネントフォルダーにコピペして、  
componentsに追加？

```
import TextareaJustHeight from './components/TextareaJustHeight'

export default {
  components: {
    TextareaJustHeight
  },
  data () {
    return {
      data: {
        text: '',
        height: '',
        length: ''
      }
    }
  }
}
```

textareaの値は `data` にbindしてくれます格納されます  
* data.height (textareaの高さ)
* data.text (入力テキスト)
* data.length (入力テキスト数)


## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# SCSSを有効化
npm install sass-loader node-sass --save-dev

<style lang="scss">
/* write SASS! */
</style>

# reset CSSをインストール
npm install --save formula-css
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
