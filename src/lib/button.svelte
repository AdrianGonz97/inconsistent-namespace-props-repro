<script lang="ts">
	export let label = "some label"
	export let disabled = false
	export let someOtherProp = 0;
	
	someOtherProp;
</script>

<button {disabled} aria-label={label}>
	<slot />
</button>