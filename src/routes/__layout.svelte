<script lang="ts">
	import '../app.css';
	import Header from '../components/Header.svelte';
</script>

<div class="bg-[#202023] min-h-screen text-[#FFFFFFEB] ">
	<div class="bg-transparent fixed w-full backdrop-filter backdrop-blur bg-opacity-50">
		<Header />
	</div>

	<div class="md:w-[800px] mx-auto flex flex-col min-h-screen">
		<div class="mx-4 md:mx-24">
			<img src="/dev.png" alt="hero" class="mx-auto mt-14" />
			<slot />
		</div>

		<footer class="text-center text-[#727274] text-sm py-10 font-semibold mt-auto">
			© 2022 Huseyin Can Soylu. All Rights Reserved.
		</footer>
	</div>
</div>
