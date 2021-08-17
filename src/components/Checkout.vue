<template>
	<div>
		<div class="container-fluid">
			<div class="row">
				<div class="col bg-dark text-white">
					<a class="navbar-brand">SPORT STORE</a>
				</div>
			</div>
		</div>
		<div class="m-2">
			<div class="form-group m-2">
				<label>Name</label>
				<input v-model="name" class="form-control" />
			</div>
		</div>
		<div class="text-center">
			<router-link to="/cart" class="btn btn-secondary m-1">
				Back
			</router-link>
			<button class="btn btn-primary m-1" v-on:click="submitOrder">
				Place Order
			</button>
		</div>
	</div>
</template>

<script>
export default {
	data: function() {
		return {
			name: null,
		};
	},
	methods: {
		submitOrder() {
			// todo: save order
		},
	},
};
</script>
