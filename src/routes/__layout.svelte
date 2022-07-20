<script lang="ts">
	import '../app.css';
	import Header from '../components/Header.svelte';
</script>

<div class="bg-[#202023] min-h-screen text-[#FFFFFFEB]">
	<div class="w-[800px] mx-auto">
		<Header />
		<slot />
		<footer class="text-center text-[#727274] text-sm py-4 font-semibold">
			© 2022 Huseyin Can Soylu. All Rights Reserved.
		</footer>
	</div>
</div>
