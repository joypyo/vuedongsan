<template>
  <div class="menu">
    <a v-for="(a) in 메뉴들" :key="a">{{a}}</a>
  
  </div>

<div v-for="test in 3" :key="test">
  <h4 >{{products[0]}}</h4>
  <p >{{price[0]}}</p>
</div>

</template>

<script>
export default {
  name: 'App',
  data(){
    return {
      메뉴들 : ['Home', 'Shop', 'About'],
      products : ['역삼동원룸', '천호동원룸', '마포구원룸'],
      price : ['70','50','30'],
    }
     
  },
  components: {
    
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
}

.menu {
  background: darkslateblue;
  padding : 15px;
  border-radius: 5px;
}
.menu a{
  color: white;
  padding: 10px;
}
</style>
