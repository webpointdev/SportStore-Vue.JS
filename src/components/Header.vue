<template>
	<div class="col bg-dark text-white" id="header">
		<a class="navbar-brand">SPORTS STORE</a>
		<cart-summary id="cart-summary" />
	</div>
</template>
<style>
#header {
	display: flex;
	justify-content: space-between;
}
.hbutton {
	padding: 5px;
}
#cart-smmary {
}
</style>
<script>
import CartSummary from "./CartSummary";
export default {
	components: { CartSummary },
};
</script>
