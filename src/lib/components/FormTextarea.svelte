<script>
	let { value = $bindable(), ...props } = $props();
</script>

<textarea class="ams-text-area" dir="auto" bind:value {...props} />
