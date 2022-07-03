<script lang="ts">
	import { lazyLoad } from '../../services/lazyLoad';
	type IPost = {
		id: number;
		title: string;
		content: string;
		createdAt: string;
		updatedAt: string;
		imageUrl: string;
	};
	export let post: IPost;
</script>

<div class="card">
	<div class="card-header">
		<div class="card-image">
			<a href="/posts/{post.id}">
				<figure class="card-image-figure lazy-container">
					<img alt="some" src="/images/loading.gif" class="lazy" use:lazyLoad={post.imageUrl} />
				</figure>
			</a>
		</div>
		<a href="/posts/{post.id}"><h3>{post.title}</h3></a>
	</div>
	<div class="card-body">
		<p>{post.content}</p>
	</div>
</div>

<style>
	.card {
		width: 100%;
	}

	figure {
		width: 100%;
		height: 150px;
	}

	img {
		width: 100%;
		height: 100%;
	}
</style>
