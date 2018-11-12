<template>
  <div id="app">
   <h1>{{title}}</h1>
   <Navbar/>
    <Blogs/>
  </div>
</template>

<script>

import Navbar from './Navbar'
import Blogs from './Blogs'

export default {
  name: 'app',
  components: {
    Navbar,
    Blogs,
  }, 
  data () {
    return {
      title: 'my first vue app, wooo :) '
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
