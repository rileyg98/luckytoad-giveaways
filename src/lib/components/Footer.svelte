<script>
	import state from '$lib/stores/fsm';
	import GiveawayTracker from './GiveawayTracker.svelte';
</script>

<footer class="flex flex-col justify-center items-center gap-10 p-8">
	{#if $state !== 'start' && $state !== 'summary'}
		<div class="flex md:hidden text-center">
			<GiveawayTracker />
		</div>
	{/if}

	<div>
		<p class="text-brand-green-dark text-xs text-center ">© Lucky Toad Team 2022. All right reserved.</p>
		<!-- <p class="text-brand-green-dark text-xs text-center ">Designed by Nick Jenkins, built by Jakub Donovan.</p> -->
	</div>
</footer>
