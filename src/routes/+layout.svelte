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
		padding-inline: var(--ams-grid-padding-inline);
		/* TODO made my own grid wrapper using the spacing var from the filesystem, must be a neater way to fix */
	}
</style>
