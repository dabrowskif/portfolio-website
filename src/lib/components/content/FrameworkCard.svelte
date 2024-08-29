<script lang="ts">
	export let icon: string;
	export let frameworkName: string;
</script>

<div class="col-span-1">
	<div class="card card-hover variant-ghost-primary">
		<header class="card-header">
			<h3 class="h5 text-center">
				{frameworkName}
			</h3>
		</header>
		<section class="p-2"></section>
		<footer class="card-footer flex justify-center">
			<img src={icon} alt="Framework Icon" class="h-12" />
		</footer>
	</div>
</div>
