<template>
	
<div id="online-friends">
	<h2>online friends</h2>
	<div v-for="(f, index) in friends" :key="index">
		<span v-if="f.online">{{f.name}}</span>
	</div>
</div>
</template>

<script>
export default {
	name: 'OnlineFriends',
	props: ['friends'],
	data() {
		return {
		
		}
	}

}
</script>

<style>


</style>
