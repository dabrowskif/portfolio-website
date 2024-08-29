<script>
	import { DotLottieSvelte } from '@lottiefiles/dotlottie-svelte';
</script>

<div id="#hero" class="grid grid-cols-6 lg:gap-10 w-full items-center">
	<div class="hidden lg:block lg:col-span-1" />
	<div class="col-span-6 md:col-span-4 md:col-start-2 lg:col-span-2 order-1 lg:order-0">
		<h1 class="text-3xl md:text-5xl lg:text-7xl">
			dabrowski<span class="text-primary-500">f</span>
		</h1>
		<h2 class="text-xl lg:text-2xl text-primary-500">rm -rf /.config/nvim</h2>
		<div class="py-5" />
		<p class="text-left text-lg md:text-xl">
			hi, i'm Filip Dąbrowski.
			<br />
			i am a backend developer located in Toruń, Poland.
			<br />
			<br />
			if you want to know a little bit more, dive in!
		</p>
	</div>

	<div class="col-span-6 md:col-span-4 md:col-start-2 lg:col-span-3 order:0 lg:order-1">
		<DotLottieSvelte src="/LaptopAnimation.json" loop autoplay />
	</div>
</div>
