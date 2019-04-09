<template>
  <div class="box">
    <textarea v-on:input="input" placeholder="テキストを入力"></textarea>
  </div>
</template>

<script>
export default {
  name: 'TextareaJustHeight',

  methods: {
    input: function () {
      this.$el.children[0].style.height = '';
      this.$el.children[0].style.height = this.$el.children[0].scrollHeight +'px';
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.box {
  margin: 0 auto;
  padding: 80px;
  width: 500px;
  background: lightgray;
  textarea {
    border: 0px;
    margin: 0px;
    padding: 10px;
    width: 400px;
    height: 45px;
    border-radius: 10px;
    color: #505050;
    resize: none;
    font-family: "メイリオ", Meiryo, monospace, "ヒラギノ角ゴ Pro W3","Hiragino Kaku Gothic Pro", YuGothic, sans-serif;
    font-size: 18px;
    line-height: 1.4;
    box-shadow: 2px 2px 0px rgba(lightgrey, 0.6) inset;
    box-sizing: border-box;
  }
}

</style>
