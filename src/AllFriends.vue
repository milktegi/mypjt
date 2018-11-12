<template>
	<div id="all-friends">
		<h2>all friends</h2>
		<div v-for="(friend, index) in friends" v-bind:key="index">
			<span>{{ friend.name }}</span>
		</div>
	</div>
</template>


<script>
export default {
	
	name: 'AllFriends',
	data() {
		return {
			friends: [
				{ name: 'mario1', online: true },
				{ name: 'mario2', online: false },
				{ name: 'mario3', online: true },
				{ name: 'mario4', online: true },
			]

		}
	}
}
</script>

<style>

</style>
