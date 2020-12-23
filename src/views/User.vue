<template>
	<div>
		<p>Usser</p>
		<button @click="add">添加</button>
	</div>
</template>

<script>
	export default{
		name: "User",
		data() {
			return {
				
			}
		},
		methods: {
			add () {
				this.$router.push('/add')
			}
		}
	}
</script>

<style>
</style>
