<!-- src/routes/+error.svelte -->
<script lang="ts">
	import { goto } from "$app/navigation";

    
</script>

<svelte:head>
	<title>Error</title>
</svelte:head>

<div class="flex h-screen flex-col items-center justify-center px-4 gap-5 text-center">
	<div class="font-mono font-semibold">Oh! You've successfully discovered the way to nothing.</div>
    <button class="bg-black px-4 py-2 rounded-md text-zinc-300" onclick={()=>{goto('/')}}>Go to Home</button>
</div>
