<script lang="ts">
	import Navbar from '$lib/components/Navbar.svelte';
</script>

<section>
	<Navbar />

	<div class="h-screen">
		<div class="mx-auto px-8 py-24 text-center md:px-12 lg:px-24 lg:pt-64">
			<div class="font-serif text-4xl font-semibold">Presenting Musicone</div>
			<div class="mb-10 font-sans text-2xl">Sync music, sync vibe with us.</div>

			<div class="group relative inline-flex items-center justify-center gap-4">
				<div
					class="transitiona-all absolute inset-0 rounded-xl bg-gradient-to-r from-indigo-500 via-pink-500 to-yellow-400 opacity-60 blur-lg filter duration-1000 group-hover:opacity-100 group-hover:duration-200"
				></div>
				<a
					role="button"
					class="group relative inline-flex items-center justify-center rounded-xl bg-gray-900 px-8 py-3 text-base font-semibold text-white transition-all duration-200 hover:-translate-y-0.5 hover:bg-gray-800 hover:shadow-lg hover:shadow-gray-600/30"
					title="payment"
					href="/"
					>Get Started For Free<svg
						aria-hidden="true"
						viewBox="0 0 10 10"
						height="10"
						width="10"
						fill="none"
						class="mt-0.5 -mr-1 ml-2 stroke-white stroke-2"
					>
						<path d="M0 5h7" class="opacity-0 transition group-hover:opacity-100"></path>
						<path d="M1 1l4 4-4 4" class="transition group-hover:translate-x-[3px]"></path>
					</svg>
				</a>
			</div>
		</div>
	</div>
	<div class="flex w-full justify-center pb-24">
		<form action="" class="w-max flex flex-col gap-4">
			<div class="group relative w-max">
				<span
					class="absolute top-2 bottom-2 -left-0.5 w-1.5 rounded bg-gradient-to-b from-indigo-500 to-purple-500 opacity-70 transition-all duration-300 group-focus-within:opacity-100"
				></span>
				<input
					type="text"
					id="input"
					placeholder=""
					class="peer w-96 rounded-lg border border-gray-200 bg-white pt-6 pr-4 pb-2 pl-6 text-sm text-gray-800 placeholder-transparent shadow-md transition-all delay-200 duration-300 focus:border-transparent focus:ring-2 focus:ring-indigo-300 focus:outline-none"
				/>
				<label
					for="input"
					class="absolute top-3.5 left-6 cursor-text text-sm text-gray-500 transition-all duration-200 ease-in-out peer-placeholder-shown:top-3.5 peer-placeholder-shown:text-base peer-placeholder-shown:text-gray-400 peer-focus:top-1 peer-focus:text-sm peer-focus:font-semibold peer-focus:text-indigo-500"
				>
					Room ID
				</label>
			</div>
			<div class="flex justify-center gap-4">
				<button
					type="submit"
					class="inline-flex min-h-[3rem] touch-manipulation items-center justify-center rounded border border-black/10 bg-white px-6 py-[calc(0.875rem-1px)] align-baseline text-base leading-tight font-semibold text-black/85 shadow-sm transition-all duration-250 select-none hover:-translate-y-px hover:border-black/15 hover:text-black/65 hover:shadow-lg focus:border-black/15 focus:text-black/65 focus:shadow-lg active:translate-y-0 active:border-black/15 active:bg-[#F0F0F1] active:text-black/65 active:shadow-md"
				>
					Create Room
				</button>
				<button
					type="submit"
					class="inline-flex min-h-[3rem] touch-manipulation items-center justify-center rounded border border-black/10 bg-white px-6 py-[calc(0.875rem-1px)] align-baseline text-base leading-tight font-semibold text-black/85 shadow-sm transition-all duration-250 select-none hover:-translate-y-px hover:border-black/15 hover:text-black/65 hover:shadow-lg focus:border-black/15 focus:text-black/65 focus:shadow-lg active:translate-y-0 active:border-black/15 active:bg-[#F0F0F1] active:text-black/65 active:shadow-md"
				>
					Join Room
				</button>
			</div>
		</form>
	</div>
</section>
