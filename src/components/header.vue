<template>
	<header class="header" id="header">
		<div class="sombra">
			<div class="container">
				<img src="img/04.png" class="rounded mx-auto d-block">
			</div>
		</div>
	</header>
</template>

<script>
export default {
	name: 'header'
}
</script>

<style>
	header{
		height: 100vh;
		background: url('../../public/img/02.jpg') center;
		background-size: cover;
	}
	header .sombra{
		display: flex;
		justify-content: center;
		height: 100vh;
		width: 100%;
		background: rgba(0,0,0,.5);
	}
	header .sombra .container{
		display: flex;
		align-items: center;
		justify-content: center;
	}
</style>