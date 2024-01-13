<script>
	export let y;

	let tabs = [
		{ name: 'Home', link: '/' },
		{ name: 'Resume', link: '/resume' },
		{ name: 'Projects', link: '/projects' },
		{ name: 'Contact', link: '/contact' }
	];
</script>

<header
	class={'sticky z-[10] top-0 duration-200 p-6 flex items-center justify-between border border-solid' +
		(y > 0 ? 'p-4 bg-slate-950 border-violet-950 ' : ' py-6 bg-transparent border-transparent ')}
>
	<h1 class="font-medium">
		<b class="font-bold poppins">João Pedro</b>
	</h1>
	<div class="sm:flex items-center gap-4 hidden">
		{#each tabs as tab, index}
			<a href={tab.link} class="duration-200 hover:text-violet-400">
				<p>{tab.name}</p>
			</a>
		{/each}
	</div>
</header>
