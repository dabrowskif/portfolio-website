<script>
	import Footer from './footer/Footer.svelte';
	import Navbar from './navbar/Navbar.svelte';
</script>

<div class="grid grid-rows-[auto_1fr_auto]">
	<header class="sticky top-0 z-10 backdrop-blur-sm p-4">
		<Navbar />
	</header>
	<main class="p-4 space-y-4 mb-10">
		<slot />
	</main>
	<Footer />
	<!-- <footer class="p-4"></footer> -->
</div>
