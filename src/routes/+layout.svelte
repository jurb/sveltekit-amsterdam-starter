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
