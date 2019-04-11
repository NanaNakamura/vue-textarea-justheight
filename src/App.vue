<template>
  <div id="app">
    <h1>input textarea just height!!!</h1>
    <div class="box">
      <TextareaJustHeight v-model="data"/>
    </div>
    <h2>data bind</h2>
    <p>data.height (textareaの高さ)<br>
    data.text (入力テキスト)<br>
    data.length (入力テキスト数)</p>
    <pre>{{ data }}</pre>
  </div>
</template>

<script>
import TextareaJustHeight from './components/TextareaJustHeight'

export default {
  name: 'App',
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
</script>

<style lang="scss" module>
@import "../node_modules/formula-css/develop/formula.scss";
</style>
<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: #2c3e50;
  margin: 100px 4%;
  h1 {
    margin-bottom: 80px;
    font-size: 2em;
    font-weight: bold;
    text-align: center;
  }
  h2 {
    margin-top: 80px;
    margin-bottom: 20px;
    font-size: 1.5em;
    font-weight: bold;
  }
  pre {
    margin-top: 20px;
    padding: 40px;
    border-radius: 6px;
    background: #f5f5f5;
  }
  p {
    word-break: break-all;
    line-height: 1.6;
  }
  .box {
    margin: 0 auto;
    padding: 80px;
    background: #eeeeee;
    + .box {
      margin-top: 80px;
    }
  }
}
</style>