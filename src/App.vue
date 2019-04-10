<template>
  <div id="app">
    <h1>input textarea just height!!!</h1>
    <TextareaJustHeight/>
  </div>
</template>

<script>
import TextareaJustHeight from './components/TextareaJustHeight'

export default {
  name: 'App',
  components: {
    TextareaJustHeight
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
}
</style>