<script>
	export let name;
	export let lastName;
	let svelteLogo = 'https://arepa.s3.amazonaws.com/svelte-logo.png'
</script>

<main>
	<h1>Hello {name} {lastName}!</h1>
	<p>Programador</p>
	<img src={svelteLogo} alt="Svelte logo">
</main>

<style>
	:global(body){
		background-color: #f2eee2;
	}

	:global(:root){
		--theme-color: rgb(15, 15, 15);
	}
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
	p {
		color: var(--theme-color);
		font-size: 22px;
	}
	main img {
		width: 30%;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>