<script context="module">
	import Splash from '$lib/Splash.svelte';
	import Grid from '$lib/Grid.svelte';
	import TwoBox from '$lib/TwoBox.svelte';
</script>

<script>
	export let splashProps;
 	export let contents;

	let webComponents = {
		grid: Grid,
		twoBox: TwoBox
	}

</script>

<Splash  {...splashProps}/>

<div class="content-wrapper">
	{#each contents as content}
		<svelte:component this={webComponents[content.name]} {...content.props} />
	{/each}
</div>
