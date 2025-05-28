<script lang="ts">
	import { onMount } from 'svelte';

	let atTop = true;
	let open = false;

	const handleScroll = () => {
		atTop = window.pageYOffset <= 50;
	};

	onMount(() => {
		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<div
	class="fixed inset-x-0 z-50 mx-auto mt-4 w-full transform rounded-full px-8 py-4 transition-all duration-1000 ease-in-out"
	class:bg-black={!atTop}
	class:bg-opacity-90={!atTop}
	class:backdrop-blur-xl={!atTop}
	class:max-w-4xl={!atTop}
	class:max-w-2xl={atTop}
>
	<div class="mx-auto flex w-full flex-col p-2 md:flex-row md:items-center md:justify-between">
		<div class="flex flex-row items-center justify-between">
			<span
				class="font-bold tracking-tighter uppercase"
				class:text-black={atTop}
				class:text-white={!atTop}
			>
				✺ Musicone
			</span>
			<button class="focus:outline-none md:hidden" on:click={() => (open = !open)}>
				<!-- Insert SVG Burger icon here -->
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke-width="1.5"
					stroke="currentColor"
					class="h-6 w-6 text-black"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						d="M3.75 5.25h16.5M3.75 12h16.5M3.75 18.75h16.5"
					/>
				</svg>
			</button>
		</div>
		<nav
			class="flex-grow flex-col justify-end gap-8 pb-4 md:flex md:flex-row md:pb-0 lg:ml-auto"
			class:flex={open}
			class:hidden={!open}
		>
			<a class:text-black={atTop} class:text-white={!atTop} href="#_">About</a>
			<a class:text-black={atTop} class:text-white={!atTop} href="#_">Contact</a>
		</nav>
	</div>
</div>
