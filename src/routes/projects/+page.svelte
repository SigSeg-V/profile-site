<script lang="ts">
	import Navbar from '$lib/components/navbar.svelte';

	const myAge = () => {
		const birthday = new Date(1999, 8, 28).getTime();
		const now = Date.now();
		const diff = now - birthday;
		return new Date(diff).getUTCFullYear() - 1970;
	};
</script>

<Navbar />

<div class="flex justify-center m-5">
	<img src="construction.png" alt="Under construction" class="max-w-sm w-1/3 rounded-lg m-2" />
</div>
