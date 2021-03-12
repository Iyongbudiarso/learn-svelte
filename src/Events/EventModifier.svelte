<!-- https://svelte.dev/tutorial/event-modifiers -->
<script>
	function handleClick() {
		alert('clicked')
	}
</script>

<button on:click|once|preventDefault={handleClick}>
	Click me
</button>
