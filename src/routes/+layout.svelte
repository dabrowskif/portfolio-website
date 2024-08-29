<script lang="ts">
	import '../app.postcss';

	// Highlight JS
	import hljs from 'highlight.js/lib/core';
	import 'highlight.js/styles/github-dark.css';
	import {
		initializeStores,
		Drawer,
		storeHighlightJs,
		getDrawerStore
	} from '@skeletonlabs/skeleton';
	import xml from 'highlight.js/lib/languages/xml'; // for HTML
	import css from 'highlight.js/lib/languages/css';
	import javascript from 'highlight.js/lib/languages/javascript';
	import typescript from 'highlight.js/lib/languages/typescript';

	hljs.registerLanguage('xml', xml); // for HTML
	hljs.registerLanguage('css', css);
	hljs.registerLanguage('javascript', javascript);
	hljs.registerLanguage('typescript', typescript);
	storeHighlightJs.set(hljs);

	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	import MainLayout from '$lib/components/layout/MainLayout.svelte';
	import MenuIcon from '$lib/icons/MenuIcon.svelte';

	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
	initializeStores();

	const drawerStore = getDrawerStore();
</script>

<Drawer position="top">
	<div class="flex justify-end">
		<button
			type="button"
			class="flex justify-center variant-ghost-primary h-10 w-10 rounded-lg"
			on:click={drawerStore.close}
		>
			<MenuIcon class="h-6 w-6  self-center" />
		</button>
	</div>
</Drawer>
<MainLayout>
	<slot />
</MainLayout>
