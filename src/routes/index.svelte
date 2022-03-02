<script>
	let count = 1;

	count++;
</script>

<div class="w-full flex flex-col sm:flex-row flex-grow overflow-hidden">
	<div class="sm:w-1/3 md:1/4 w-full flex-shrink flex-grow-0 p-4">
		<div class="sticky top-0 p-4 w-full">
			<ul class="flex sm:flex-col overflow-hidden content-center justify-between">nav</ul>
		</div>
	</div>
	<main class="w-full h-full flex-grow p-3 overflow-auto">
		<h1>Welcome to SvelteKit</h1>
		<p on:click={(e) => count++}>
			Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
			{count}
		</p>
	</main>
</div>
<footer class="mt-auto">footer</footer>
