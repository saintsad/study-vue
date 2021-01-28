<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="어떻게 이렇게 바뀌지?"/>
    <A2 url="http://www.naver.com">네이버</A2>
    <hr/>
    <input type="text" v-model="title" />
    <div>{{title2}}</div>
    <hr/>
    <button id="show-modal" @click="showModal = true">Show Modal</button>
    <Modal v-if="showModal" @close="showModal = false">
      <div slot="body">dsfdsfsdf<br/> dsfdsfdsf<br/> dsfdsfsdfsdfdsfdsfdsf</div>
      <h1 slot="header">{{title}}</h1>
    </Modal>
    
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import A2 from './components/A2.vue'
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    A2,
    Modal
  },
  data(){
    return {
      title: '',
      showModal : false
    }
  },
  computed: {
    title2:function(){
      return this.title+'원'
    }
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
