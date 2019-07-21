<template>
  <div id="app">
    <p>{{count}}</p>
    <input type="button" value="点我+" @click="add">
    <input type="button" value="点我-" @click="sub">
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  data(){
    return{
      count:0
    };
  },
  methods:{
    add(){
      this.count++;
    },
    sub(){
      this.count--;
    }
  },
  components: {
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
