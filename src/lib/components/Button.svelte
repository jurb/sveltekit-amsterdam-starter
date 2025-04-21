<script lang="ts">
	let { onclick = undefined, children } = $props();
</script>

<button class="ams-button ams-button--primary" type="button" {onclick}>{@render children()}</button>
