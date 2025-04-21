<script>
	import '../main.css';
	import Header from '$lib/components/Header.svelte';
	let { children } = $props();
</script>

<Header appTitle="Test app" />

<div class="grid-wrapper ams-screen ams-screen--wide">
	<div class="ams-grid">
		<div class="ams-grid__cell ams-grid__cell--span-all">
			{@render children()}
		</div>
	</div>
</div>

<style>
	.grid-wrapper {
		background-color: #f5f5f5;
		min-height: 100vh; /* Make it at least full viewport height */
		width: 100%;
	}
</style>