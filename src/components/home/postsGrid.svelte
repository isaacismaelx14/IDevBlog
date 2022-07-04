<script lang="ts">
	import Card from '../common/card.svelte';
	export let posts: IPost[] = [];
</script>

{#if posts.length > 0}
	<div class="grid">
		{#each posts as post}
			<Card {post} />
		{/each}
	</div>
{:else}
	<div class="centered">
		<h2>I'm coding awesome ideas to post right here!</h2>
		<small>(Meanwhile you can see more about me <a href="https://isaacmartinez.dev">here</a>)</small
		>
	</div>
{/if}

<!-- <div class="grid">
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/388x150'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/388x150'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/388x150'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/388x150'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/388x150'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/388x150'
		}}
	/>
</div> -->
<style>
	.centered {
		width: 100%;
		height: 150px;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
	}

	.grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
		grid-gap: 20px;
		margin-top: 20px;
	}

	h2 {
		font-weight: 300;
		font-size: 22px;
		text-align: center;
	}

	small {
		color: #848484;
	}

	a {
		color: var(--primary-color-light);
		text-decoration: none;
	}
</style>
