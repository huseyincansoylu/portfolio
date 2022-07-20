<script lang="ts">
	export let studyAndExperience: any[];
</script>

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
