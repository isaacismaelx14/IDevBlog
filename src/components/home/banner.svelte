<script lang="ts">
	import { config } from '../../config/config';
	let appTitle = config.app_name;
</script>

<div>
	<h2>Welcome to <strong>{appTitle}</strong></h2>
</div>

<style>
	div {
		width: 100%;
		height: 30vh;
		display: flex;
		align-items: center;
		justify-content: center;
		background-color: var(--secondary-color);
		color: #000;
	}

	h2 {
		font-size: 2rem;
		font-weight: 300;
		color: var(--primary-color-light);
	}

	strong {
		color: var(--primary-color);
	}

	@media (min-width: 801px) {
		div {
			height: 40vh;
		}

		h2 {
			font-size: 3rem;
		}
	}
</style>
