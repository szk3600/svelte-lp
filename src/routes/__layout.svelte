<script>
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/purecss@2.0.6/build/pure-min.css" integrity="sha384-Uu6IeWbM+gzNVXJcM9XV3SohHtmWE+3VGi496jvgX1jyvDTXfdK+rfZc8C1Aehk5" crossorigin="anonymous">
	<link rel="stylesheet" href="https://unpkg.com/purecss@2.0.6/build/grids-responsive-min.css">
  <link rel="stylesheet" href="https://netdna.bootstrapcdn.com/font-awesome/4.0.3/css/font-awesome.css">
  <link rel="stylesheet" href="/lp-style.css">
</svelte:head>


<div class="header">
    <div class="home-menu pure-menu pure-menu-horizontal pure-menu-fixed">
       <a class="pure-menu-heading" href="/">Your Site</a>

        <ul class="pure-menu-list">
            <li class="pure-menu-item pure-menu-selected"><a href="/" class="pure-menu-link">Home</a></li>
            <li class="pure-menu-item"><a href="/" class="pure-menu-link">Tour</a></li>
            <li class="pure-menu-item"><a href="/" class="pure-menu-link">Sign Up</a></li>
        </ul>
    </div>
</div>


<main>
	<slot />
</main>

