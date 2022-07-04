<script lang="ts">
	import { config } from '../../config/config';
	let appTitle = config.app_name;
</script>

<header>
	<div class="container">
		<h2>
			<a href="/" class="logo">{appTitle}</a>
		</h2>
	</div>
</header>

<style>
	header {
		background-color: var(--primary-color);
		height: var(--header-height);
		width: 100%;
		display: flex;
		align-items: center;
	}

	.container {
		align-content: center;
		display: flex;
		justify-content: space-between;
	}

	a {
		color: #fff;
		text-decoration: none;
	}
</style>
