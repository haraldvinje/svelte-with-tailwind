<script context="module" lang="ts">
	export const prerender = true;
</script>

<script lang="ts">
	import Counter from '$lib/Counter.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="prose lg:prose-xl flex flex-col items-center">
	<div>
		<picture>
			<source srcset="svelte-welcome.webp" type="image/webp" />
			<img src="svelte-welcome.png" alt="Welcome" />
		</picture>
	</div>

	<h1 >
		to your new<br />SvelteKit app
	</h1>

	<h2>
		try editing <strong>src/routes/index.svelte</strong>
	</h2>
	<Counter />
</section>