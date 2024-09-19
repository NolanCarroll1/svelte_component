<script>
	export let yes = false;
</script>

<label class="text-gray-100">
	<input type="checkbox" bind:checked={yes}  />
	Yes! Send me regular email spam
</label>

{#if yes}
	<p class="text-gray-100">Thank you. We will bombard your inbox and sell your personal details.</p>
{:else}
	<p class="text-gray-100">You must opt-in to continue. If you're not paying, you're the product.</p>
{/if}