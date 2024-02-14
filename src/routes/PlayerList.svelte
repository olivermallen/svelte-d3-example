<script>
	// data comes from the load function in +page.js
	export let dataset;
</script>

<div class="container">
</div>

<ul>
{#each dataset as player}
<li>{player.name} ({player.team})</li>
{/each}
</ul>

<style>
    ul {
        list-style: none;
        padding: 0;
    }
    li+li {
        margin-top: 0.5em

    }
</style>
