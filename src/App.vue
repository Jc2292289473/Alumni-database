<template>
  <div id="app">
    <navigation/>
    <mybody/>
    <test/>
  </div>
</template>

<script>
import navigation from './components/navigation.vue'
import test from './components/test.vue'
import mybody from './components/mybodys.vue'

export default {
  name: 'App',
  components: {
    navigation,
    test,
    mybody,
  }
}
</script>

<style>
body{
  margin: 0px;
  background: rgb(230, 235, 242) 
}
</style>
