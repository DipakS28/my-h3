<script lang="ts">
	import { duckDbInstance } from '$lib/duckdbInstanceStore';
	import '../app.css';
</script>

<div class="w-full h-full grid grid-rows-[auto_1fr_auto]">
	<main class="w-full h-full py-2 pt-12 p-3 container mx-auto overflow-auto">
		{#if $duckDbInstance.isInstantiated}
			<slot></slot>
		{/if}
	</main>
</div>

