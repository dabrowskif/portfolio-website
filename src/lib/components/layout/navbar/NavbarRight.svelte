<!-- NavbarRight.svelte -->
<script lang="ts">
	import MenuIcon from '$lib/icons/MenuIcon.svelte';
	import type { DrawerSettings } from '@skeletonlabs/skeleton';
	import { getDrawerStore } from '@skeletonlabs/skeleton';

	const drawerSettings: DrawerSettings = {
		bgDrawer: 'variant-filled-surface border border-primary-500',
		bgBackdrop: 'bg-gradient-to-b from-black/90 to-primary-900/20',
		width: 'w-full',
		height: 'h-full sm:h-[500px]',
		padding: 'p-4',
		rounded: 'rounded-xl'
	};
	const drawerStore = getDrawerStore();
</script>

<div class="flex gap-5 items-center">
	<a href="https://github.com/dabrowskif" target="_blank" aria-label="GitHub Profile">
		<img src="/github.png" alt="Github Icon" class="h-9" />
	</a>
	<a href="https://www.linkedin.com/in/dabrowskif/" target="_blank" aria-label="LinkedIn Profile">
		<img src="/linkedin.svg" alt="LinkedIn Icon" class="h-10" />
	</a>
	<button
		type="button"
		class="flex justify-center variant-ghost-primary h-10 w-10 transition-all duration-150 rounded-lg"
		on:click={() => drawerStore.open(drawerSettings)}
		aria-label="Menu"
	>
		<MenuIcon class="h-6 w-6 self-center" />
	</button>
</div>
