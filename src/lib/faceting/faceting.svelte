<script>
	import Dailies from '$lib/dailies/dailies.svelte';

	let max_nodes = 8;

	let advantage_rows = [[1], []];
	let disadvantage_row = [];
</script>

<div class="w-8/12 p-6">
	{#each advantage_rows as adv_row}
		<div class="flex justify-between py-4">
			{#each [...Array(max_nodes).keys()] as node}
				{#if node >= adv_row.length}
					<div class="bg-gray-500 h-2 w-2 inline-block mr-2" />
				{:else}
					<div
						class:bg-red-400={!adv_row[node]}
						class:bg-blue-400={adv_row[node]}
						class="h-2 w-2 inline-block mr-2"
					/>
				{/if}
			{/each}
		</div>
	{/each}
</div>
