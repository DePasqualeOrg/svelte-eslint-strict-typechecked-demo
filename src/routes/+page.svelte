<script lang="ts">
	const emptyString = '';

	// This results in an error due to @typescript-eslint/no-unnecessary-condition
	if (emptyString) {
		console.log('test');
	}
</script>

<!-- This does not result in an error -->
{#if emptyString}
	<p>test</p>
{/if}
