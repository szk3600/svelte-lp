<script context="module">	import { browser, dev } from '$app/env';	export const hydrate = dev;	export const router = browser;	export const prerender = true;	import LP from '$lib/LP.svelte';</script>

<script>
	import lpProps from '$lib/data/lp/tama.json';
</script>
<LP {...lpProps} />


