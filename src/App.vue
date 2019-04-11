<template>
  <div id="app">
    <h1>input textarea just height!!!</h1>
    <div class="box">
      <TextareaJustHeight v-model="data"/>
    </div>
    <div class="box ta-l">
      <h2>data bind</h2>
      <h3>data.text (入力テキスト)</h3>
      <p>→　{{ data.text }}</p>
      <h3>data.height (textareaの高さ)</h3>
      <p>→　{{ data.height }}</p>
      <h3>data.length (入力テキスト数)</h3>
      <p>→　{{ data.length }}</p>
    </div>
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
  text-align: center;
  color: #2c3e50;
  margin: 100px 4%;
  h1 {
    margin-bottom: 80px;
    font-size: 2em;
    font-weight: bold;
  }
  h2 {
    margin-bottom: 20px;
    font-size: 1.5em;
    font-weight: bold;
  }
  h3 {
    margin-top: 20px;
    // margin-bottom: 10px;
    font-size: 1em;
    font-weight: bold;
  }
  .box {
    margin: 0 auto;
    padding: 80px;
    width: 80%;
    background: lightgray;
    + .box {
      margin-top: 80px;
    }
    p {
      word-break: break-all;
      line-height: 1.6;
    }
  }
  .ta-l {
    text-align: left;
  }
}
</style>