<template>
  <div id="app">
   <h1>{{title}}</h1>
   <Navbar/>
  </div>
</template>

<script>

import Navbar from './Navbar'


export default {
  name: 'app',
  components: {
    Navbar: Navbar
  }, 
  data () {
    return {
      title: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>


h1, h2 {
  color:rgb(88, 88, 204);
  font-weight: normal;

}


</style>
