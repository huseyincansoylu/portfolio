<script lang="ts">
	export let studyAndExperience: any[];
	export let title: string;
</script>

<div class="mt-10">
	<h4 class="text-xl font-semibold border-b-2 pb-2 border-[#4DAE9D] inline-block">{title}</h4>

	{#each studyAndExperience as education}
		<div class="mt-6">
			<div class="flex justify-between">
				<div class="flex-1 ">
					<p class="font-semibold">{education.name}</p>
					<p class="italic mt-1">{education.field}</p>
				</div>
				<p>{education.time}</p>
			</div>
		</div>
	{/each}
</div>
