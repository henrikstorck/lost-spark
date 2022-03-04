<script>
	import { page } from '$app/stores';

	export let path;
	export let name;
</script>

<li>
	<a
		href={path}
		class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 {$page.url.pathname == path
			? 'text-white bg-blue-700 rounded md:rounded-none md:text-white md:bg-transparent'
			: 'hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-400 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent'} dark:border-gray-700"
		aria-current="page">{name}</a
	>
</li>
