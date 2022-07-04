<script lang="ts">
	import Header from '../components/common/header.svelte';
</script>

<Header />
<main>
	<slot />
</main>

<style global>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	:root {
		--header-height: 60px;
		--primary-color: rgb(27, 38, 50);
		--primary-color-light: rgb(57, 80, 104);
		--secondary-color: rgb(227, 227, 227);
	}

	body {
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell,
			'Open Sans', 'Helvetica Neue', sans-serif;
	}

	main {
		width: 100%;
		overflow: auto;
		height: calc(100vh - var(--header-height));
	}

	.container {
		width: 100%;
		padding: 0 30px;
	}

	.lazy {
		width: 70px !important;
		height: 70px !important;
	}

	.lazy-container {
		display: flex;
		justify-content: center;
		align-items: center;
	}

	@media (min-width: 768px) {
		.container {
			padding: 0 80px;
		}
	}
</style>
