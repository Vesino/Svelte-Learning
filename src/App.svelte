<script>
	// Components
	import About from './components/About.svelte'
	import Counter from './components/Counter.svelte'
	import Person from './components/Person.svelte'

	// Variables
	export let name;
	export let lastName;
	let svelteLogo = 'https://arepa.s3.amazonaws.com/svelte-logo.png'
	let data = {
		name: 'Vesino',
		lastName: 'Vargas',
		age: 27
	}
</script>

<main>
	<h1>{name} {lastName}!</h1>
	<About />
	<Counter />
	<Person { ...data }/>
	<img src={svelteLogo} alt="Svelte logo">
</main>

<style>
	:global(body){
		background-color: #f2eee2;
	}

	:global(:root){
		--theme-color: rgb(15, 15, 15);
	}

	:global(body.dark-mode){
		background-color: #1d3040;
		color: #bfc2c7;
	}
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
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