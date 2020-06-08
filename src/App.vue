<template>
    <div id="app">
        <barra />
        <datos v-bind:ruta="this.ruta"/>
        <router-view/>
    </div>
</template>

<script>
import barra from '@/components/nav-bar.vue'
import datos from '@/components/data-bar.vue'

export default {
	components:{
		barra,
		datos
	},
	data(){
		return{
			ruta: this.$route.path
		}
	}
}
</script>

<style>

</style>
