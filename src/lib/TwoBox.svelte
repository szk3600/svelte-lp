<script>
	import Box from './Box.svelte';
	export let title;
	export let box1;
	export let box2;
</script>

<div class="content">
  <h2 class="content-head is-center">{title}</h2>
	<Box {...box1} />
	<Box {...box2} />
</div>
