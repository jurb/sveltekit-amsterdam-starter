<script>
	import '../main.css';
	import Header from '$lib/components/Header.svelte';
	let { children } = $props();
</script>

<div class="ams-screen ams-screen--wide ams-docs-screen">
	<div class="ams-grid">
		<div class="ams-grid__cell ams-grid__cell--span-all">
			<Header appTitle="Test app" />
		</div>
		<div class="ams-grid__cell ams-grid__cell--span-all">
			<div class="wrapper">
				{@render children()}
			</div>
		</div>
	</div>
</div>

<style>
	.wrapper {
		padding-inline: var(--ams-header-padding-inline);
		/* TODO: haha we use the same padding var as used in the header to pad the app wrapper, NOT the way */
	}
</style>
