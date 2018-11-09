<template>
  <div id="app">
    <div class="app_header">
     <Header></Header>
    </div>
    <div class="nav">
      <div class="nav-item">
        <a link="{path:'/goods'}">商品</a>
        
      </div>
      <div class="nav-item">
        <a link="{path:'/ratings'}">评论</a>
        
      </div>
      <div class="nav-item">
        <a v-link="{path:'/seller'}">商家</a>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<script>
import Header from './components/header/header.vue'
export default {
  name: 'App',
  components:{
    Header
  }
}
</script>

<style rel="./common/style/reset.css">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#app .nav{
  display: flex;
  width: 100%;
  height: 40px;
  line-height: 40px;
}
#app .nav .nav-item{
  flex: 1;
  text-align: center;
}

</style>
