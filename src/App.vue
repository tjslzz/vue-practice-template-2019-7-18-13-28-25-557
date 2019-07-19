<template>
  <div id="app">
    <p>{{counter}}</p>
    <button @click="counter ++">点我+</button>
    <button @click="counter --">点我-</button>
    <button @click="extra">抽方法</button>
  </div>
</template>

<script>
export default {
  name: 'app',
  data:function(){
    return {
      counter : 0
    }
  },
  methods:{
    extra : function(){
      this.counter == "抽方法" ? this.counter = 0 : this.counter = "抽方法";
    }
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
