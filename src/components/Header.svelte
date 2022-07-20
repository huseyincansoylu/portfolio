<script lang="ts">
	import GithubIcon from './icons/GithubIcon.svelte';
	import Sun from './icons/Sun.svelte';
	import Code from './icons/Code.svelte';
</script>

<div class="p-2 flex items-center">
	<div class="font-semibold text-lg cursor-pointer flex items-center">
		<Code />
		<span class="ml-1">Huseyin Can Soylu</span>
	</div>
	<div class="mr-auto flex items-center ml-8 space-x-8 mt-0.5">
		<div class="cursor-pointer hover:underline">Works</div>
		<div class="flex items-center cursor-pointer hover:underline">
			<GithubIcon />
			<span class="pl-1">Source</span>
		</div>
	</div>
	<div
		class="bg-[#FBD38D] h-10 w-10 rounded-md flex items-center justify-center text-black cursor-pointer hover:bg-[#F6AD55]"
	>
		<Sun />
	</div>
</div>
