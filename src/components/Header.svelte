<script lang="ts">
	import GithubIcon from './icons/GithubIcon.svelte';
	import Sun from './icons/Sun.svelte';
	import Code from './icons/Code.svelte';
	import Moon from './icons/Moon.svelte';
	import { darkMode } from '../store';

	function toggleDarkMode() {
		if ($darkMode === true) {
			document.documentElement.classList.remove('dark');
			darkMode.set(false);
		} else {
			document.documentElement.classList.add('dark');
			darkMode.set(true);
		}
	}
</script>

<div class="md:w-[800px] mx-auto backdrop-filter backdrop-blur">
	<div class="p-4 md:p-2 flex items-center">
		<a href="/" class="font-semibold text-lg cursor-pointer flex items-center">
			<Code />
			<span class="ml-1">Huseyin Can Soylu</span>
		</a>
		<div class="mr-auto flex items-center ml-8 space-x-8 mt-0.5">
			<a href="/works" class="hidden md:inline-block cursor-pointer hover:underline">Works</a>
			<div class="hidden md:flex items-center cursor-pointer hover:underline">
				<GithubIcon />
				<a href="https://github.com/huseyincansoylu/portfolio" target="_blank" class="pl-1"
					>Source</a
				>
			</div>
		</div>
		<div
			on:click={toggleDarkMode}
			class="bg-[#6B46C1] dark:bg-[#FBD38D] h-10 w-10 rounded-md flex items-center justify-center text-white dark:text-black cursor-pointer dark:hover:bg-[#F6AD55]"
		>
			{#if $darkMode}
				<Sun />
			{:else}
				<Moon />
			{/if}
		</div>
	</div>
</div>
