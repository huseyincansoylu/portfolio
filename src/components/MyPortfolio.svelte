<script lang="ts">
	import ArrowRight from './icons/ArrowRight.svelte';
</script>

<div class="w-full flex flex-col items-center md:flex-row mt-10">
	<div class="flex-1 flex flex-col items-center md:block">
		<h1 class="text-4xl font-semibold">Huseyin Can Soylu</h1>
		<button>
			<a
				href="/works"
				class="px-4 py-2 rounded-md bg-[#67C8B7] dark:bg-[#4DAE9D] mt-6 font-semibold flex items-center"
				>My portfolio <span class="ml-2 md:mt-1"><ArrowRight /></span>
			</a>
		</button>
	</div>

	<div class="w-28">
		<img class="mt-8 md:mt-0 rounded-full border-2 border-gray-300" src="/canpg.jpg" alt="" />
	</div>
</div>
