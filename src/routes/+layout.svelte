<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<header>
	<h1>Codemere</h1>
	<h2>Enjoy the journey, celebrate the destination</h2>
</header>

<nav>
	<ul>
		<li><a href="#">Blogs</a></li>
		<li><a href="#">About</a></li>
	</ul>
</nav>
{@render children()}

<style>
	:global(body) {
		background-color: #2c2b3c;
	}
</style>
