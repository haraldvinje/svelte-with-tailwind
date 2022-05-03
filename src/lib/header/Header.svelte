<script lang="ts">
	import { page } from '$app/stores';
	const style = "px-2 py-2 rounded-md transition ease-in-out duration-200 hover:text-black hover:bg-white"
	const activeTabStyle = "text-black bg-white"
</script>

<header class="flex py-8 bg-black text-white text-xl font-bold">
	<nav class="grow">
		<ul class="flex justify-center items-center space-x-32">
			<li>
				<a sveltekit:prefetch href="/">
					<span class={`${style} ${$page.url.pathname === '/' ? activeTabStyle : ''}`}>
						Home
					</span>
				</a>
			</li>
			<li>
				<a sveltekit:prefetch href="/about">
					<span class={`${style} ${$page.url.pathname === '/about' ? activeTabStyle : ''}`}>
						About
					</span>
				</a>
			</li>
			<li>
				<a sveltekit:prefetch href="/todos">
					<span class={`${style} ${$page.url.pathname === '/todos' ? activeTabStyle : ''}`}>
						Todos
					</span>
				</a>
			</li>
		</ul>
	</nav>
</header>