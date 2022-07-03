<header>
	<div class="container">
		<h1>
			<a href="/" class="logo"> MyBlog </a>
		</h1>
		<nav>
			<ul>
				<li>
					<a href="/about">About</a>
				</li>
				<li>
					<a href="/blog">Blog</a>
				</li>
			</ul>
		</nav>
	</div>
</header>

<style>
	header {
		background-color: rgb(23, 23, 23);
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

	nav {
		height: 100%;
		margin: auto 0;
	}
	ul {
		display: flex;
		gap: 10px;
	}

	li {
		list-style: none;
	}
</style>
