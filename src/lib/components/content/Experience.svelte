<script>
	import Container from '../layout/main/Container.svelte';
	import ExperienceCard from './ExperienceCard.svelte';
</script>

<Container id="experience">
	<h2 class="h1 text-center mb-5">
		experienc<span class="text-primary-500">e</span>
	</h2>

	<div class="flex flex-col gap-5 mt-10">
		<ExperienceCard
			company="NCU in Toruń"
			description="engineer's degree in computer science"
			fromYear="October 2017"
			toYear="October 2021"
		/>
		<ExperienceCard
			company="Hintech"
			description="fullstack development, working mainly in React, Next.js, backend workers (web scrapping, data parsing, STT transcriptions) in Node.js, as well as writing REST API and integrating Stripe payments."
			fromYear="May 2022"
			toYear="May 2023"
		/>
		<ExperienceCard
			company="Husaria Solutions"
			description="building frontend website for private client using React, Next.js and Tailwind"
			fromYear="June 2023"
			toYear="October 2023"
		/>
		<ExperienceCard
			company="Footballco"
			description="implementing GraphQL API with NestJS, AWS and Terraform for sports data pages and CMS"
			fromYear="July 2023"
			toYear="now"
		/>
	</div>
</Container>
