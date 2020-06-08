<template>
	<div class="data" id="data">
		<h4 class="subtitle is-6">{{ month }} {{ day }} of {{ year }} {{ ruta }}</h4>
		<hr>
	</div>
</template>

<script>
export default{
	data(){
		return {
			month: Date().split(' ')[1],
			day: Date().split(' ')[2],
			year: Date().split(' ')[3]
		}
	},
	computed:{
		hour: () => {
			return Date().split(' ')[4];
		}
	},
	name: 'data',
	props:{
		ruta: String
	}
}
</script>

<style>
	.data{
		display: flex;
		z-index: 1;
		position: absolute;
		bottom: 0;
	}
	hr{
		background: #f5f5f5;
		height: 2px;
		width: 100px;
		border: none;
	}
	h4{
		color: #f5f5f5 !important;
		padding: 15px;
		margin: 0 !important;
	}
	h4:hover{
		color: aqua !important;
		cursor: pointer;
	}
	hr:hover{
		background: aqua;
	}
</style>