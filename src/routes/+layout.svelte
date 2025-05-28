<script lang="ts">
	import '../app.css';

	let { children } = $props();
</script>

<div class="min-h-screen bg-gradient-to-l from-gray-200 via-fuchsia-200 to-stone-100">
	{@render children()}
</div>
