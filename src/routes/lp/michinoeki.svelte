<script context="module">	import { browser, dev } from '$app/env';	export const hydrate = dev;	export const router = browser;	export const prerender = true;	import LP from '$lib/LP.svelte';</script><script>

	let grid = 			{ name: 'grid',
										props: {
											title: 'Grid Component',
					items: [
						{
							icon: 'fa fa-rocket',
							title: 'Get Started Quickly',
							text: 'Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.'
						},
						{
							icon: 'fa fa-mobile',
							title: 'Responsive Layouts',
							text: 'Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.'
						},
						{
							icon: 'fa fa-th-large',
							title: 'Modular',
							text: 'Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.'
						},
						{
							icon: 'fa fa-check-square-o',
							title: 'Play Well',
							text: 'Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.'
						}
					]
				}
											};
	let twoBox = { name: 'twoBox',
								 props: {
									 title: 'Tow Box Component',
									 box1:	{
										 icon: 'fa fa-rocket',
										 title: 'Get Started Quickly',
										 text: 'Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.'
									 },
									 box2:	{
										 icon: 'fa fa-mobile',
										 title: 'Responsive Layouts',
										 text: 'Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.'
									 }
								 }
							 };



	let lpProps = {
		splashProps: {
			head: "道の駅",
			subHead: "道の駅で、楽しくお食事や休憩をしましょう！",
			href: "http://purecss.io",
			buttonText: "行ってみよう！",
		},
		contents: [
			grid,twoBox,			grid,twoBox
		]
	};

</script><LP {...lpProps} />


