<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="어떻게 이렇게 바뀌지?"/>
    <A2 url="http://www.naver.com">네이버</A2>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import A2 from './components/A2.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    A2
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
