<script>
	let questions = [
		{ id: 1, text: `Start` },
		{ id: 2, text: `Stop` },
		{ id: 3, text: `clone` }
	];

	let selected;

	let answer = '';

	function handleSubmit() {
		alert(`answered question ${selected.id} (${selected.text}) with "${answer}"`);
	}
</script>


	<select value={selected} on:change="{() => answer = ''}">
		{#each questions as question}
			<option value={question}>
				{question.text}
			</option>
		{/each}
	</select>

	

<style>
	input {
		display: block;
		width: 500px;
		max-width: 100%;
	}
</style>