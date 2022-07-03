<script lang="ts">
	import Card from '../common/card.svelte';
</script>

<div class="grid">
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/240x150'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/250x120'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/240x150'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/250x120'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/240x150'
		}}
	/>
	<Card
		post={{
			content: 'lorem ipsum',
			title: 'Lorem',
			createdAt: '',
			id: 12,
			updatedAt: '',
			imageUrl: 'https://via.placeholder.com/250x120'
		}}
	/>
</div>

<style>
	.grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
		grid-gap: 20px;
		margin-top: 20px;
	}
</style>
