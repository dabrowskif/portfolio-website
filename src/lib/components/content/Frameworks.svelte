<script>
	import Container from '../layout/main/Container.svelte';
	import FrameworkCard from './FrameworkCard.svelte';

	const javascriptIconPath = '/javascript.svg';
	const typescriptIconPath = '/typescript.svg';
	const golangIconPath = '/golang.svg';

	const nestjsIconPath = '/nestjs.svg';
	const svelteIconPath = '/svelte.svg';
	const reactIconPath = '/react.svg';
	const nextjsIconPath = '/nextjs.svg';
	const tailwindIconPath = '/tailwind.svg';

	const nodeIconPath = '/node.svg';

	const dynamodbIconPath = '/dynamodb.svg';
	const postgresqlIconPath = '/postgresql.svg';
	const mongodbIconPath = '/mongodb.svg';
	const drizzleIconPath = '/drizzle';

	const awsIconPath = '/aws.svg';
	const terraformIconPath = '/terraform.svg';
	const supabaseIconPath = '/supabase.svg';
	const cloudflareIconPath = '/cloudflare.svg';
	const githubIconPath = '/github.png';
	const dockerIconPath = '/docker.svg';

	const sectionClass = 'grid grid-cols-2 lg:grid-cols-4 gap-10 my-10';
</script>

<Container id="frameworks">
	<h2 class="h1 text-center mb-10">my techstac<span class="text-primary-500">k</span></h2>
	<h3 class="h3 text-center underline decoration-primary-500">languages</h3>
	<p class="text-center">i know, node is a runtime...</p>
	<div class={sectionClass}>
		<FrameworkCard icon={javascriptIconPath} frameworkName="Javascript" />
		<FrameworkCard icon={typescriptIconPath} frameworkName="Typescript" />
		<FrameworkCard icon={nodeIconPath} frameworkName="Node.js" />
		<FrameworkCard icon={golangIconPath} frameworkName="Go" />
	</div>

	<h3 class="h3 text-center underline decoration-primary-500">frameworks</h3>
	<p class="text-center">because why to reinvent the wheel?</p>
	<div class={sectionClass}>
		<FrameworkCard icon={nestjsIconPath} frameworkName="NestJS" />
		<FrameworkCard icon={svelteIconPath} frameworkName="SvelteKit" />
		<FrameworkCard icon={nextjsIconPath} frameworkName="Next.js" />
		<FrameworkCard icon={tailwindIconPath} frameworkName="Tailwind" />
	</div>

	<h3 class="h3 text-center underline decoration-primary-500">libraries</h3>
	<p class="text-center">i just had to do it, for the memes</p>
	<div class={sectionClass}>
		<FrameworkCard icon={reactIconPath} frameworkName="React" />
	</div>

	<h3 class="h3 text-center underline decoration-primary-500">databases</h3>
	<p class="text-center mb-10 italic">**quip has been stored successfully**</p>
	<div class={sectionClass}>
		<FrameworkCard icon={postgresqlIconPath} frameworkName="PostgreSQL" />
		<FrameworkCard icon={dynamodbIconPath} frameworkName="DynamoDB" />
		<FrameworkCard icon={mongodbIconPath} frameworkName="MongoDB" />
		<FrameworkCard icon={drizzleIconPath} frameworkName="Drizzle" />
	</div>

	<h3 class="h3 text-center underline decoration-primary-500">and some others</h3>
	<p class="text-center mb-10">just in case my home server has a bad day</p>
	<div class={sectionClass}>
		<FrameworkCard icon={awsIconPath} frameworkName="AWS" />
		<FrameworkCard icon={cloudflareIconPath} frameworkName="Cloudflare" />
		<FrameworkCard icon={terraformIconPath} frameworkName="Terraform" />
		<FrameworkCard icon={supabaseIconPath} frameworkName="Supabase" />
		<FrameworkCard icon={githubIconPath} frameworkName="Github" />
		<FrameworkCard icon={dockerIconPath} frameworkName="Docker" />
	</div>
</Container>
