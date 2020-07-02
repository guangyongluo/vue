<template>
	<div id="app">
		<h1>welcome to suzhou</h1>
		<h2 @click="change">{{name}}</h2>
		
		<user-list></user-list>
	</div>
</template>

<script>
	
	//导入模块
	import User from './components/User.vue';
	
	// console.log(111);
	export default {
		data(){
			return{
				name: 'tom'
			}
		},
		methods: {
			change(){
				this.name = '汤姆';
			}
		},
		components: {
			'user-list':User
		}
	}
</script>

<style>
	body {
		background-color: #ccc;
	}
</style>
