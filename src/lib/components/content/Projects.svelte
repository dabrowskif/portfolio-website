<script>
	import Container from '../layout/main/Container.svelte';
	import ProjectCard from './ProjectCard.svelte';
</script>

<Container id="projects">
	<h2 class="h1 text-center mb-5">
		project<span class="text-primary-500">s</span>
	</h2>
	<p class="text-center">i believe this is the most important part of every passionate developer</p>

	<div class="flex flex-col gap-5 mt-10">
		<ProjectCard
			name="typed routes"
			description="library enabling type-safe, file-based routing for Meta frameworks like SvelteKit or Next.js. It traverses the file tree and generates a typed object with correct segments specific to the chosen framework."
			githubLink="https://github.com/dabrowskif/typed-routes"
			npmLink="https://www.npmjs.com/package/@dabrowskif/typed-routes"
		/>
		<ProjectCard
			name="shopping lister"
			description="simple app for aggregating recipes and generating shopping lists. Ideal for personal use and meal planning. Check out the source code or visit the live site"
			githubLink="https://github.com/dabrowskif/shopping-lister"
			websiteLink="https://shopping-lister.dabrowskif.com"
		/>
		<ProjectCard
			name="kloniecki"
			description="business portfolio website built with SvelteKit, designed to showcase a professional service"
			githubLink="https://github.com/dabrowskif/kloniecki"
			websiteLink="https://kloniecki.pl"
		/>
		<ProjectCard
			name="znajdź zwierzaka"
			description="web app featuring a breeding profile browser engine, acting as a semi-social platform with marketplace functionalities. Coming soon!"
		/>
	</div>
</Container>
