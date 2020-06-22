<template>
	<div id="app">
		<barra />
		<datos/>
		<pagination v-bind:items="this.all" v-bind:ruta="this.ruta"/>
		<!-- <h4 v-for="item in all" :key="item">
			{{item}}
		</h4> -->
		<header class="header" id="header">
			<div class="sombra">
				<router-view/>
			</div>
		</header>
	</div>
</template>

<script>
import barra from '@/components/nav-bar.vue'
import datos from '@/components/data-bar.vue'
import pagination from '@/components/pagination.vue'

export default {
	components:{
		barra,
		datos,
		pagination
	},
	data(){
		return{
			ruta: this.$route,
			all: this.$router.options.routes
		}
	}
}
</script>

<style>
header{
	height: 100vh;
	background: url('../public/img/02.jpg') center;
	background-size: cover;
}
header .sombra{
	display: flex;
	justify-content: center;
	height: 100vh;
	width: 100%;
	background: rgba(0,0,0,.5);
}
</style>
