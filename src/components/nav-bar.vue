<template>
	<nav class="nav navbar is-fixed-top" role="navigation" aria-label="main navigation" id="nav">
		<div class="container">
			<div class="navbar-brand">
				<router-link to="/" class="navbar-item title is-5">Coffe <svg class="bi bi-cup" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor">
  <path fill-rule="evenodd" d="M12 4H4v8a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1V4zM3 3v9a2 2 0 0 0 2 2h6a2 2 0 0 0 2-2V3H3z"/>
  <path fill-rule="evenodd" d="M14.5 5.5h-2v-1h2A1.5 1.5 0 0 1 16 6v4a1.5 1.5 0 0 1-1.5 1.5h-2v-1h2a.5.5 0 0 0 .5-.5V6a.5.5 0 0 0-.5-.5z"/>
</svg></router-link>
			</div>
			<div class="navbar-end">
				<router-link to="/About" class="navbar-item">
				<svg class="bi bi-person" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor">
					<path fill-rule="evenodd" d="M13 14s1 0 1-1-1-4-6-4-6 3-6 4 1 1 1 1h10zm-9.995-.944v-.002.002zM3.022 13h9.956a.274.274 0 0 0 .014-.002l.008-.002c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664a1.05 1.05 0 0 0 .022.004zm9.974.056v-.002.002zM8 7a2 2 0 1 0 0-4 2 2 0 0 0 0 4zm3-2a3 3 0 1 1-6 0 3 3 0 0 1 6 0z"/>
				</svg>
				About</router-link>
				<router-link to="/" class="navbar-item"><svg class="bi bi-card-text" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor">
  <path fill-rule="evenodd" d="M14.5 3h-13a.5.5 0 0 0-.5.5v9a.5.5 0 0 0 .5.5h13a.5.5 0 0 0 .5-.5v-9a.5.5 0 0 0-.5-.5zm-13-1A1.5 1.5 0 0 0 0 3.5v9A1.5 1.5 0 0 0 1.5 14h13a1.5 1.5 0 0 0 1.5-1.5v-9A1.5 1.5 0 0 0 14.5 2h-13z"/>
  <path fill-rule="evenodd" d="M3 5.5a.5.5 0 0 1 .5-.5h9a.5.5 0 0 1 0 1h-9a.5.5 0 0 1-.5-.5zM3 8a.5.5 0 0 1 .5-.5h9a.5.5 0 0 1 0 1h-9A.5.5 0 0 1 3 8zm0 2.5a.5.5 0 0 1 .5-.5h6a.5.5 0 0 1 0 1h-6a.5.5 0 0 1-.5-.5z"/>
</svg> Contact</router-link>
			</div>
		</div>
	</nav>
</template>
<script>
export default {
	name: 'nav-bar',
	props: {}
}
</script>
<style>
	nav{
		position: fixed;
		background: transparent !important;
	}
	a{
		color: #f5f5f5 !important;
	}
	a:hover{
		background: transparent !important;
		color: aqua !important;
	}

</style>