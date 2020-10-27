<template>
  <div id="app">
    <!--img src="./assets/logo.png"--->
    <!--router-view/--->
    {{title}}
    <!--hild v-on:changeTitle="updateText($event)"/-->
    <Login/>
  </div>
</template>

<script>
import Login from './components/Login'
export default {
  name: 'App',
  components:{
    Login
  },
  data(){
    return{
      title:"Chils to parent"
    }
  },
  methods:{
    updateText(title){
      this.title=title;
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
