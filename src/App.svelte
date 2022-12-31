<script>
	import Nested from "./Conditionals/Nested.svelte";
	import Info from './Conditionals/Info.svelte';
	import Conditionals from "./Conditionals.svelte";

	const pkg = {
		name: 'svelte',
		version: 3,
		speed: 'blazing',
		website: 'https://svelte.dev'
	};
</script>

<Nested answer={42}/>
<Nested />

<Info name={pkg.name} version={pkg.version} speed={pkg.speed} website={pkg.website}/>
<Info {...pkg} />

<Conditionals />