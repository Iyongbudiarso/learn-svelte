<script>
import DomEventForwardingButton from "./DomEventForwardingButton.svelte";

function handleClick() {
	alert('clicked');
}
</script>

<DomEventForwardingButton on:click={handleClick}/>
