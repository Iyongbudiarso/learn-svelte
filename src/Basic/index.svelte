<script>
	import Component from './Component.svelte';

	export let name;

	let src = 'favicon.png';
	let nameImage = 'svelte';

	let string = `this string contains some <strong>HTML!!!</strong>`;
</script>

<h1>Hello {name}!</h1>
<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>

<img {src} alt="{nameImage} logo">
<Component />

<p>{@html string}</p>

<style>
	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	p {
		color: purple;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>
