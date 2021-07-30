<script>
	export let head;
	export let subHead;
	export let href;
	export let buttonText;
</script>

<div class="splash-container">
    <div class="splash">
        <h1 class="splash-head">{head}</h1>
        <p class="splash-subhead">{subHead} </p>
        <p>
            <a href="{href}" class="pure-button pure-button-primary">{buttonText}</a>
        </p>
    </div>
</div>
