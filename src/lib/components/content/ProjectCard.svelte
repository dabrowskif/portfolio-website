<script lang="ts">
	import EyeIcon from '$lib/icons/EyeIcon.svelte';

	export let name: string;
	export let description: string;
	export let githubLink: string = '';
	export let npmLink: string = '';
	export let websiteLink: string = '';
</script>

<div class="col-span-1">
	<div class="card card-hover variant-ghost-primary">
		<header class="card-header flex justify-between">
			<h3 class="h2 text-primary-500">
				{name}
			</h3>
			<div class="flex items-center gap-5">
				<div>
					{#if npmLink}
						<a href={npmLink} target="_blank">
							<img src="/npm.svg" alt="NPM Icon" class="h-6 sm:h-10 mt-2" />
						</a>
					{:else if websiteLink}
						<a href={websiteLink} target="_blank">
							<EyeIcon class="text-4xl sm:text-6xl" />
						</a>
					{/if}
				</div>
				<div>
					{#if githubLink}
						<a href={githubLink} target="_blank">
							<img src="/github.png" alt="Github Icon" class="h-8 sm:h-12" />
						</a>
					{/if}
				</div>
			</div>
		</header>
		<section class="mt-4"></section>
		<footer class="card-footer">
			<p class="text-sm">
				{description}
			</p>
		</footer>
	</div>
</div>
