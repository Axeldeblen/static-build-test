<script>
	import { page } from '$app/stores';
	import { onMount } from 'svelte';

	onMount(() => {
		console.log('mount');
		console.log($page.url.searchParams.toString());
		console.log($page.url.searchParams.get('tag'));
	});
</script>

<h1>Welcome to SvelteKit</h1>
<a href="/new/?tag=navigated">tag = navigated</a>
