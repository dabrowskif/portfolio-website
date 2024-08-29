<script>
	import Container from '../layout/main/Container.svelte';
	import ProjectCard from './ProjectCard.svelte';
</script>

<Container id="#projects">
	<h2 class="h1 text-center mb-5">
		project<span class="text-primary-500">s</span>
	</h2>
	<p class="text-center">i believe this is the most important part of every passionate developer</p>

	<div class="flex flex-col gap-5 mt-10">
		<ProjectCard
			name="typed routes"
			description="library allowing type-safe file-based routing for Meta frameworks like Sveltekit or Next.js. traverses the filetree and generates typed object with correct segments specific to chosen framework."
			githubLink="https://github.com/dabrowskif/typed-routes"
			npmLink="https://www.npmjs.com/package/@dabrowskif/typed-routes"
		/>
		<ProjectCard
			name="shopping lister"
			description="simple app for aggregating recipes and generating shopping lists for personal purpose. click the eye above!"
			githubLink="https://github.com/dabrowskif/typed-routes"
			websiteLink="https://shopping-lister.dabrowskif.com"
		/>
		<ProjectCard
			name="kloniecki"
			description="business portfolio website built in SvelteKit"
			githubLink="https://github.com/dabrowskif/typed-routes"
			websiteLink="https://kloniecki.pl"
		/>
		<ProjectCard
			name="znajdź zwierzaka"
			description="web app with breeding profile browser engine. Semi-social app with marketplace purposes that I’m willing to push live in the near future."
		/>
	</div>
</Container>
