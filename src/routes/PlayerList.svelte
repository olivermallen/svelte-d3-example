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
    li+li {
        margin-top: 0.5em
    }
</style>
