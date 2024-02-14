<script>
	import './style.css';
	import PlayerList from "./PlayerList.svelte";

	// data comes from the load function in +page.js
	export let data;

	// default features to visualize
	let xFeature = 'strikeout';
	let yFeature = 'hit';
	let colorFeature = 'all_star';
</script>

<div class="container">
	<div class="main">
		<PlayerList dataset = {data.dataset} />
	</div>
</div>

<style>
	.container {
		/* set the font */
		font-family: system-ui, sans-serif;
		font-size: 16px;
	}
</style>
