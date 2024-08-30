<script lang="ts">
	import CloseIcon from '$lib/icons/CloseIcon.svelte';
	import { getDrawerStore } from '@skeletonlabs/skeleton';
	import { onMount } from 'svelte';

	const drawerStore = getDrawerStore();

	onMount(() => {
		document.addEventListener('keydown', (event) => {
			if (event.key === 'Escape') {
				drawerStore.close();
			}
		});
	});
</script>

<div class="flex flex-col h-full bg-primary-900 text-white justify-between">
	<div class="flex justify-end mb-6">
		<button
			type="button"
			class="flex justify-center h-10 w-10 rounded-lg"
			on:click={drawerStore.close}
		>
			<CloseIcon class="h-6 w-6  self-center" />
		</button>
	</div>

	<nav class="flex-1 p-6">
		<ul class="space-y-4">
			<li>
				<a
					href="#hero"
					class="text-2xl font-semibold hover:underline"
					on:click={() => drawerStore.close()}>home</a
				>
			</li>
			<li>
				<a
					href="#frameworks"
					class="text-2xl font-semibold hover:underline"
					on:click={() => drawerStore.close()}>tech stack</a
				>
			</li>
			<li>
				<a
					href="#projects"
					class="text-2xl font-semibold hover:underline"
					on:click={() => drawerStore.close()}>projects</a
				>
			</li>
			<li>
				<a
					href="#experience"
					class="text-2xl font-semibold hover:underline"
					on:click={() => drawerStore.close()}>experience</a
				>
			</li>
		</ul>
	</nav>

	<div class="mt-6 p-6 br-red-500">
		<p class="text-lg font-medium">connect with me:</p>
		<div class="flex gap-4 mt-2">
			<a href="https://github.com/dabrowskif" target="_blank" aria-label="GitHub">
				<img src="/github.png" alt="GitHub Icon" class="h-8" />
			</a>
			<a href="https://www.linkedin.com/in/dabrowskif/" target="_blank" aria-label="LinkedIn">
				<img src="/linkedin.svg" alt="LinkedIn Icon" class="h-8" />
			</a>
		</div>

		<footer class="mt-6 text-sm">
			<p>© 2024 Filip Dąbrowski</p>
		</footer>
	</div>
</div>
