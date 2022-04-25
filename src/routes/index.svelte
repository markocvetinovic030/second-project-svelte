<script>
	import Header from '../components/header.svelte';
	import Main from '../components/main.svelte';
	import Tabs from '../shered/tabs.svelte';

	let items = ['Home', 'About', 'Contact'];
	let activeItem = 'Home';
	const tabChange = (e) => {
		activeItem = e.detail;
	};
</script>

<div class="scroll-smooth">
	<Tabs {activeItem} {items} on:tabChange={tabChange} />
	{#if activeItem === 'Home'}
		<Header />
		<Main />
	{:else if activeItem === 'About'}
		<Header />
	{:else if activeItem === 'Contact'}
		<Header />
		<p>car</p>
	{/if}
</div>
