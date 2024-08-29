<script lang="ts">
	export let id: string = '';
</script>

{#if id}
	<div {id} class="max-w-2xl mx-auto">
		<slot />
	</div>
{:else}
	<div class="max-w-2xl mx-auto">
		<slot />
	</div>
{/if}
