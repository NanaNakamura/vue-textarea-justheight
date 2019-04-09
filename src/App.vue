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

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  h1 {
    margin-bottom: 80px;
  }
}
</style>
