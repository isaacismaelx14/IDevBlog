<script lang="ts">
	import { lazyLoad } from '../../services/lazyLoad';
	export let post: IPost;
</script>

<div class="card">
	<div class="card-header">
		<div class="card-image">
			<a href="/posts/{post.Id}">
				<figure class="card-image-figure lazy-container">
					<img alt="some" src="/images/loading.gif" class="lazy" use:lazyLoad={post.ImageUrl} />
				</figure>
			</a>
		</div>
		<a href="/posts/{post.Id}"><h3>{post.Title}</h3></a>
	</div>
	<div class="card-body">
		<p>{post.Body}</p>
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
