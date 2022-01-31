<script>
	import { page } from '$app/stores';
	import { onMount } from 'svelte';

	onMount(() => {
		console.log('mount');
		console.log($page.url.searchParams.toString());
		console.log($page.url.searchParams.get('tag'));
	});
</script>

<a href="/?tag=backToHome">tag = backToHome</a>
