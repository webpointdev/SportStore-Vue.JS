<template>
	<div class="col bg-dark text-white" id="header">
	<div class="nav">
		<a class="navbar-brand">SPORTS STORE</a>
	</div>
	<div class="nav hbutton">
		<button type="button" class="navbar-brand btn btn-info"
		v-on:click="adddata"
		>ADD SOTRE DATA</button>
		<button type="button" v-on:click="deldata" class="navbar-brand btn btn-info">DELETE SOTRE DATA</button>
	</div>
	</div>
</template>
<style>
#header{
	display:flex;
	justify-content:space-between;
}
.hbutton{
	padding:5px;
}
</style>
<script>
		export default {
		methods: {
			adddata(){
				alert("success!");
			},
			deldata(){
				alert("choose select!");
			}
		}
	}
</script>