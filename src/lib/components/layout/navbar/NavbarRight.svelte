<script lang="ts">
	// import LightIcon from '$lib/icons/LightIcon.svelte';
	import MenuIcon from '$lib/icons/MenuIcon.svelte';
	import type { DrawerSettings } from '@skeletonlabs/skeleton';
	import { getDrawerStore } from '@skeletonlabs/skeleton';

	const drawerSettings: DrawerSettings = {
		id: 'example-3',
		// Provide your property overrides:
		bgDrawer: 'variant-filled-surface border border-primary-500',
		bgBackdrop: 'bg-gradient-to-tr from-primary-400/20 via-primary-600/20 to-primary-900/20',
		width: 'w-full',
		height: 'h-1/4',
		padding: 'p-4',

		rounded: 'rounded-xl'
	};
	const drawerStore = getDrawerStore();
</script>

<div class="flex gap-5">
	<a href="https://github.com/dabrowskif" target="_blank" class="m-auto">
		<img src="/github.png" alt="Github Icon" class="h-9" />
	</a>
	<a href="https://www.linkedin.com/in/dabrowskif/" target="_blank">
		<img src="/linkedin.svg" alt="LinkedIn Icon" class="h-10" />
	</a>
	<!-- <button -->
	<!-- 	type="button" -->
	<!-- 	class="flex justify-center variant-ghost border border-primary-500 h-10 w-10" -->
	<!-- > -->
	<!-- 	<LightIcon class="h-6 w-6 self-center" /> -->
	<!-- </button> -->
	<button
		type="button"
		class:rounded-lg={$drawerStore.open}
		class="flex justify-center variant-ghost-primary h-10 w-10 transition-all duration-150"
		on:click={() => drawerStore.open(drawerSettings)}
	>
		<MenuIcon class="h-6 w-6  self-center" />
	</button>
</div>
