<template>
	<div class="cont">
		<span v-for="item in this.items" :key="item" :class="{ inpage: item.path == ruta.fullPath}">
		</span>
	</div>
</template>

<script>
export default{
	name: 'pagination',
	data(){
		return {

		}
	},
	props:{
		items: Array,
		ruta: String
	}
}
</script>

<style>
	.cont{
		position: absolute;
		background: transparent;
		top: 50%;
		color: #f5f5f5;
		padding: 10px;
	}
	.cont span{
		display: block;
		height: 7px;
		width: 7px;
		background: rgba(255,255,255,.8);
		margin: 5px;
		border-radius: 50%;
	}
	span.inpage{
		height: 10px;
		width: 10px;
	}

</style>