<script>
	import { page } from '$app/stores';
	import LinkIcon from '../../components/icons/LinkIcon.svelte';
	import { projects } from '../../data';

	const { id } = $page.params;
	const project = projects.find((project) => project.id === parseInt(id));
</script>

<svelte:head>
	<title>{project?.name} - Huseyin Can Soylu</title>
</svelte:head>
{#if project}
	<div>
		<div class="flex justify-center">
			<h4 class="text-white bg-[#C75183] px-2 py-1 font-semibold rounded-md">
				{project?.name.toUpperCase()}
			</h4>
		</div>

		<p class="mt-6 italic tracking-wide">{project.info || project.desc}</p>
		<div class="py-4 space-y-2 my-2">
			<div class="flex items-center">
				<span
					class="text-green-300 font-semibold bg-green-300 bg-opacity-30 px-2 rounded-md text-sm"
					>REPO</span
				>
				<a
					href={project.repo}
					target="_blank"
					class="hidden md:block pl-2 text-base text-orange-300 hover:underline">{project.repo}</a
				>
				<a
					href={project.repo}
					target="_blank"
					class="md:hidden pl-2 text-base text-orange-300 underline underline-offset-4"
					>go to repo</a
				>
				<span class="pl-1"><LinkIcon /></span>
			</div>

			<div class="flex items-center">
				<span
					class="text-green-300 font-semibold bg-green-300 bg-opacity-30 px-2 rounded-md text-sm"
					>WEBSITE</span
				>
				<a
					href={project.link}
					target="_blank"
					class="hidden md:block pl-2 text-base text-orange-300 hover:underline">{project.link}</a
				>
				<a
					href={project.link}
					target="_blank"
					class="md:hidden pl-2 text-base text-orange-300 underline underline-offset-4"
					>go to website</a
				>
				<span class="pl-1"><LinkIcon /></span>
			</div>
			<div class="flex items-center">
				<span
					class="text-green-300 font-semibold bg-green-300 bg-opacity-30 px-2 rounded-md text-sm"
					>TECH</span
				>
				<span class="text-orange-300 pl-2 ">{project.tech}</span>
			</div>
		</div>

		<div class="grid grid-cols-1  gap-6">
			{#each project.src as item}
				<img src={item} alt="project-showcase" class="object-contain rounded-xl" />
			{/each}
		</div>
	</div>
{:else}
	<p class="text-center">No project with this id:{id}</p>
{/if}
