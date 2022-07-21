<script>
	import HomeSlot from '../components/HomeSlot.svelte';
</script>

<HomeSlot title="Projects">
	<div class="grid grid-cols-2 mt-6 gap-4">
		<div>
			<img src="/wordle1.png" alt="" class="object-contain rounded-xl cursor-pointer" />
			<h5 class="text-center font-semibold mt-4 cursor-pointer ">Wordle Clone</h5>
		</div>
		<div>
			<img src="/jobify1.png" alt="" class="object-contain rounded-xl cursor-pointer" />
			<h5 class="text-center font-semibold mt-4 cursor-pointer">Jobify</h5>
		</div>
		<div>
			<img src="/twitter1.png" alt="" class="object-contain rounded-xl cursor-pointer" />
			<h5 class="text-center font-semibold mt-4 cursor-pointer">Twitter Clone</h5>
		</div>
	</div>
</HomeSlot>
