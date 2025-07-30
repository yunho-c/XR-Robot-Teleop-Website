<script>
	let { tabs } = $props();
	let selected = Object.keys(tabs)[0];
</script>

<div class="tabs-container">
	<ul class="tabs-list">
		{#each Object.keys(tabs) as name}
			<li on:click={() => (selected = name)} class:active={selected === name}>
				<span role="button" tabindex="0">{name}</span>
			</li>
		{/each}
	</ul>
	<div class="tab-content">
		{@render tabs[selected]()}
	</div>
</div>

<style>
	.tab-content {
		margin-bottom: 10px;
		padding: 40px;
		border: 1px solid #dee2e6;
		border-radius: 0 0 0.5rem 0.5rem;
		border-top: 0;
	}
	.tabs-list {
		display: flex;
		flex-wrap: wrap;
		padding-left: 0;
		margin-bottom: 0;
		list-style: none;
		border-bottom: 1px solid #dee2e6;
	}
	.tabs-list li {
		margin-bottom: -1px;
	}

	.tabs-list li span {
		border: 1px solid transparent;
		border-top-left-radius: 0.25rem;
		border-top-right-radius: 0.25rem;
		display: block;
		padding: 0.5rem 1rem;
		cursor: pointer;
	}

	.tabs-list li span:hover {
		border-color: #e9ecef #e9ecef #dee2e6;
	}

	.tabs-list li.active > span {
		color: #495057;
		background-color: #fff;
		border-color: #dee2e6 #dee2e6 #fff;
	}
</style>
