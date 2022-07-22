<script>
	import HomeSlot from '../../components/HomeSlot.svelte';
	import { projects } from '../../data';
</script>

<svelte:head>
	<title>Works - Huseyin Can Soylu</title>
</svelte:head>
<HomeSlot title="Projects">
	<div class="grid grid-cols-1 md:grid-cols-2 mt-6 gap-4">
		{#each projects as project (project.id)}
			<div>
				<a href={`/works/${project.id}`}>
					<img
						src={project.src[0]}
						alt="project-showcase"
						class="object-contain rounded-xl cursor-pointer"
					/>
				</a>
				<h5 class="text-center font-semibold mt-4 ">{project.name}</h5>
				<div class="text-center mt-2">
					<span class="text-sm">{project.desc}</span>
				</div>
			</div>
		{/each}
	</div>
</HomeSlot>
