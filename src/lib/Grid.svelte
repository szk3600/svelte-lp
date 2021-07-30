<script>
	import Box from './Box.svelte';
	export let title;
	export let items;
</script>

<div class="content">
  <h2 class="content-head is-center">{title}</h2>
	{#each items as item}
		<Box {...item} />
	{/each}
</div>
