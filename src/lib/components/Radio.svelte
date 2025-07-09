<script lang="ts">
	let { value = $bindable(), children } = $props();
</script>

<div class="ams-radio">
	<input name="about" class="ams-radio__input" id=":r15:" type="radio" bind:value />
	<label class="ams-radio__label" for=":r15:">
		<span class="ams-radio__icon-container">
			<svg
				aria-hidden="true"
				focusable="false"
				viewBox="0 0 24 24"
				xmlns="http://www.w3.org/2000/svg"
			>
				<circle class="ams-radio__circle" cx="12" cy="12" r="10"></circle>
				<circle class="ams-radio__hover-indicator" cx="12" cy="12" r="9.5"></circle>
				<circle class="ams-radio__checked-indicator" cx="12" cy="12" r="6"></circle>
			</svg>
		</span>
		{@render children()}
	</label>
</div>
