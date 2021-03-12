<script>
	import Outer from './ComponentEventOuter.svelte';

	function handleMessage(event) {
		alert(event.detail);
	}
</script>

<Outer on:message={handleMessage}/>
