<script lang="ts">
	import Post from '$lib/domain/posts/Post.svelte';

	let posts = $state([
		{
			id: 1,
			title: 'Post 1',
			description: 'This is a test',
			date: '2026-01-20',
			category: 'Random'
		},
		{
			id: 2,
			title: 'Post 2',
			description: 'This is a test',
			date: '2026-01-20',
			category: 'Algorithm'
		},
		{
			id: 3,
			title: 'Post 3',
			description: 'This is a test',
			date: '2026-01-20',
			category: 'Opinion'
		}
	]);
</script>

{#each posts as post (post.id)}
	<Post title={post.title} date={post.date} category={post.category} />
{/each}
