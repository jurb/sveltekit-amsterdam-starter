<script>
	import Radio from './Radio.svelte';
	let radioGroup = $state('');
</script>

group: {radioGroup}

<fieldset aria-describedby="description1" role="radiogroup" class="ams-field-set">
	<legend class="ams-field-set__legend">Waar gaat uw melding over?</legend>
	<p class="ams-paragraph ams-paragraph--small ams-mb-s" id="description1">
		De laatstgenoemde melding.
	</p>
	<div class="ams-column ams-column--gap-x-small">
		<Radio value="horeca" bind:group={radioGroup}>Horeca</Radio>
		<div class="ams-radio">
			<input name="about" class="ams-radio__input" id=":r16:" type="radio" value="ander_bedrijf" />
			<label class="ams-radio__label" for=":r16:">
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
				Ander soort bedrijf
			</label>
		</div>
		<div class="ams-radio">
			<input name="about" class="ams-radio__input" id=":r17:" type="radio" value="evenement" />
			<label class="ams-radio__label" for=":r17:">
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
				Evenement
			</label>
		</div>
		<div class="ams-radio">
			<input name="about" class="ams-radio__input" id=":r18:" type="radio" value="anders" />
			<label class="ams-radio__label" for=":r18:">
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
				Iets anders
			</label>
		</div>
	</div>
</fieldset>
