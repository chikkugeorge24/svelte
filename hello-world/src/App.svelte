<script>
	const name = 'Chikku George'
	const channel = '<b>Crafts Grimoire</b>'
	const hack = `<a href="#" onClick="alert('You have been hacked')">Win a prize</a>`
	const id = 'heading'
	const disabled = true
</script>

<main>
	<h1>Hello {name}</h1>
	<div>{@html channel}</div>
	<div>{@html hack}</div>
	<h1 {id}>This is a heading</h1>
	<button {disabled}>Bind</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>