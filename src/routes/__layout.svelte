<script lang="ts">
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
</script>

<div class="flex flex-col min-h-screen">
	<Header />

	<main class="flex min-h-[50%] justify-center my-16 mx-32">
		<slot />
	</main>

	<footer class="prose lg:prose-xl bg-slate-300 flex justify-center items-center flex-grow min-h-[20rem] min-w-full">
		<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p>
	</footer>
</div>