<template>
  <div id="app">
   <h1>{{title}}</h1>
   <Navbar/>
   <AllFriends :friends="friends" @delete="deleteFriend"/>
   <OnlineFriends :friends="friends"/>
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
      title: 'Welcome to Your Vue.js App',
      	friends: [
				{ name: 'mario1', online: true },
				{ name: 'mario2', online: false },
				{ name: 'mario3', online: true },
				{ name: 'mario4', online: false },
			]

    }
  },
  methods: {
    deleteFriend(payload) {
      this.friends = this.friends.filter(friend => {
        return friend.name !== payload.name;
      })
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
