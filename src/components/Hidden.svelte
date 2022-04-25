<script>
	export let shown = false;

	export const show = () => {
		shown = !shown;
	};
</script>

<button
	class="bg-white w-16 h-16 rounded-full mt-10 block m-auto hover:animate-bounce hover:mt-12"
	on:click={show}><img class="w-8 m-auto" src="../src/image/download.png" alt="down" /></button
>

{#if shown}
	<slot />
{/if}
