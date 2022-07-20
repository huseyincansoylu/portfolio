<script lang="ts">
	import GithubIcon from './icons/GithubIcon.svelte';
	import Sun from './icons/Sun.svelte';
	import Code from './icons/Code.svelte';
</script>

<div class="p-4 md:p-2 flex items-center">
	<a href="/" class="font-semibold text-lg cursor-pointer flex items-center">
		<Code />
		<span class="ml-1">Huseyin Can Soylu</span>
	</a>
	<div class="mr-auto flex items-center ml-8 space-x-8 mt-0.5">
		<a href="/works" class="hidden md:inline-block cursor-pointer hover:underline">Works</a>
		<div class="hidden md:flex items-center cursor-pointer hover:underline">
			<GithubIcon />
			<a href="https://github.com/huseyincansoylu/portfolio" target="_blank" class="pl-1">Source</a>
		</div>
	</div>
	<div
		class="bg-[#FBD38D] h-10 w-10 rounded-md flex items-center justify-center text-black cursor-pointer hover:bg-[#F6AD55]"
	>
		<Sun />
	</div>
</div>
