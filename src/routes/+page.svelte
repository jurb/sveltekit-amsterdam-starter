<script>
	import Button from '$lib/components/Button.svelte';
	import FormField from '$lib/components/FormField.svelte';
	import FormLabel from '$lib/components/FormLabel.svelte';
	import FormTextarea from '$lib/components/FormTextarea.svelte';
	import FormInput from '$lib/components/FormInput.svelte';
	let formInputA = $state('');
	let formInputB = $state('');
	let aantalRuns = $state(10);
</script>

<p class="ams-paragraph--large">
	Niet meer naar het Stadsloket, maar thuis of op het werk uw nieuwe paspoort ontvangen. In juni en
	juli kan dat. Deze zomer bezorgt de gemeente reisdocumenten gratis aan huis. We doen dat om de
	drukte in de Stadsloketten te verminderen. En u hoeft maar 1 keer naar het Stadsloket.
</p>

<p>
	<strong>formInputA</strong>: {formInputA}
</p>
<p>
	<strong>formInputB</strong>: {formInputB}
</p>
<p>
	<strong>aantalRuns</strong>: {aantalRuns}
</p>


<p><a href="./test"><Button>link test</Button></a></p>
<p><Button onclick={() => console.log('haai')}>log on click</Button></p>

<div class="form-columns-wrapper">
	<div class="form-column">
		<FormField>
			<FormLabel>
				<h3 style="margin-block-end: 0">Variant A</h3>
				<p class="ams-paragraph"><strong>Zuidoost</strong></p>
			</FormLabel>
			<FormTextarea bind:value={formInputA}></FormTextarea>
		</FormField>
	</div>
	<div class="form-column">
		<FormField>
			<FormLabel>
				<h3 style="margin-block-end: 0">Variant B</h3>
				<p class="ams-paragraph"><strong>Zuid</strong></p>
			</FormLabel>
			<FormTextarea bind:value={formInputB}></FormTextarea>
		</FormField>
	</div>
</div>
<p>Aantal runs: <FormInput bind:value={aantalRuns} type="number" /> </p>
<p><Button onclick={() => console.log('haai')}>Vergelijking runnen</Button></p>

<style>
	.form-columns-wrapper {
		display: flex;
		gap: 1rem;
		width: 100%;
	}

	.form-column {
		flex: 1;
	}
</style>
