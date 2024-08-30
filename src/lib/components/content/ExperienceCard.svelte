<script lang="ts">
	export let company: string;
	export let description: string;
	export let fromYear: string;
	export let toYear: string;
</script>

<div class="col-span-1">
	<div class="card card-hover variant-ghost-primary">
		<header class="card-header flex flex-col sm:flex-row justify-between">
			<h3 class="h4 text-primary-500">
				{company}
			</h3>
			<p class="h-6 md:h4 underline decoration-primary-500">{fromYear} - {toYear}</p>
		</header>
		<section class="p-1"></section>
		<footer class="card-footer">
			<p class="text-sm">
				{description}
			</p>
		</footer>
	</div>
</div>
