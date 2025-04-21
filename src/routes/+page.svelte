<script>
	import Button from '$lib/components/Button.svelte';
	import FormField from '$lib/components/FormField.svelte';
	import FormLabel from '$lib/components/FormLabel.svelte';
	import FormTextarea from '$lib/components/FormTextarea.svelte';
	import FormInput from '$lib/components/FormInput.svelte';
	let formInputText = $state('');
	let formInputNumbers = $state(10);
</script>

<p class="ams-paragraph--large">
	Niet meer naar het Stadsloket, maar thuis of op het werk uw nieuwe paspoort ontvangen. In juni en
	juli kan dat. Deze zomer bezorgt de gemeente reisdocumenten gratis aan huis. We doen dat om de
	drukte in de Stadsloketten te verminderen. En u hoeft maar 1 keer naar het Stadsloket.
</p>

<p>
	<strong>formInputText</strong>: {formInputText}
</p>
<p>
	<strong>formInputNumbers</strong>: {formInputNumbers}
</p>

<p><a href="./test"><Button>link test</Button></a></p>
<p><Button onclick={() => console.log('haai')}>log on click</Button></p>

<FormField>
	<FormLabel>
		<h3 style="margin-block-end: 0">Form</h3>
		<p class="ams-paragraph">Explanatory text</p>
		<!-- TODO: there are components / styles for form text elements, not implemented here -->
	</FormLabel>
	<FormTextarea bind:value={formInputText}></FormTextarea>
</FormField>

<p>Here is a number: <FormInput bind:value={formInputNumbers} type="number" /></p>
<p><Button onclick={() => console.log('send demo')}>Versturen</Button></p>

<style>
</style>
