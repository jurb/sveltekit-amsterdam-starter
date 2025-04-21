<script>
	let { value = $bindable(), ...props } = $props();
</script>

<input class="ams-text-input" dir="auto" type="text" bind:value {...props} />
