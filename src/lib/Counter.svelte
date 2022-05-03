<script lang="ts">
	let count = 0;
</script>

<div class="flex flex-grow py-2 px-2 my-2 rounded-md border-2 border-black gap-x-4 text-2xl">
	<button 
		class="bg-red-500 text-white px-4" 
		on:click={() => (count -= 1)} 
	>
		-
	</button>

	<div class="counter-viewport">
		<strong>{count}</strong>
	</div>

	<button 
		class="bg-green-500 text-white px-4" 
		on:click={() => (count += 1)}
	>
		+
	</button>
</div>