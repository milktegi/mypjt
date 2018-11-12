<template>
  <div id="app">
   <h1>{{title}}</h1>
   <Navbar/>
   <AllFriends/>
   <OnlineFriends/>
  </div>
</template>

<script>

import Navbar from './Navbar'
import AllFriends from './AllFriends'
import OnlineFriends from './OnlineFriends'


export default {
  name: 'app',
  components: {
    Navbar,
    AllFriends,
    OnlineFriends
  }, 
  data () {
    return {
      title: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style scoped>


h1, h2 {
  color:rgb(88, 88, 204);
  font-weight: normal;

}


</style>
