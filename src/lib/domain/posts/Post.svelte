<script lang="ts">
	let { title, date, category } = $props();
</script>

<div class="post">
	<h1 class="post__title">{title}</h1>

	<div class="post__info">
		<h2 class="post__date">{date}</h2>
		<h2 class="post__category">{category}</h2>
	</div>
</div>

<style>
	.post {
		display: flex;
		justify-content: space-between;
		padding: 0.75rem;
		margin-bottom: 0.5rem;
		font-size: 12px;
		border: 1px solid white;
		color: #ffffff;
		background-color: #201f30;
	}
	.post__info {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		line-height: 0;
		font-size: 9px;
	}
</style>
