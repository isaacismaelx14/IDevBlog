<script lang="ts">
	import PostsGrid from '../components/home/postsGrid.svelte';
	import Banner from '../components/home/banner.svelte';
	import { config } from '../config/config';
	let appTitle = config.app_name;
</script>

<svelte:head>
	<title>{appTitle} | home</title>
	<meta name="description" content="Blog for developers about tips, news and more." />
</svelte:head>

<div class="container">
	<Banner />
	<PostsGrid />
</div>
