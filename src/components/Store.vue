<template>
	<div class="container-fluid">
		<div class="row">
			<Header />
		</div>
		<div class="row">
			<div class="col-3 bg-info p-2">
				<CategoryControls class="mb-5" />
				<button
					class="btn btn-block btn-warning mt-5"
					v-on:click="setShowSearch(true)"
				>
					Search
				</button>
			</div>
			<div class="col-9 p-2">
				<Search />
				<ProductList />
			</div>
		</div>
		<div class="row">
			<Footer />
		</div>
	</div>
</template>
<script>
import Vue from "vue";
import Vuex from "vuex";
Vue.use(Vuex);
import ProductList from "./ProductList";
import CategoryControls from "./CategoryControls";
import Header from "./Header";
import Footer from "./Footer";
import Search from "./Search";
import { mapMutations } from "vuex";
export default {
	components: { Header, Footer, ProductList, CategoryControls, Search },
	methods: {
		...mapMutations(["setShowSearch"]),
	},
};
</script>
