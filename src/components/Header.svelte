<script lang="ts">
	import GithubIcon from './icons/GithubIcon.svelte';
	import Code from './icons/Code.svelte';
	import { page } from '$app/stores';

	$: isRootWorks = $page.routeId === 'works';
</script>

<div class="md:w-[800px] mx-auto backdrop-filter backdrop-blur">
	<div class="p-4 md:p-2 flex items-center">
		<a href="/" class="font-semibold text-lg cursor-pointer flex items-center">
			<Code />
			<span class="ml-1">Huseyin Can Soylu</span>
		</a>
		<div class="ml-auto flex items-center space-x-8 mt-0.5">
			<a
				href="/works"
				class={`underline-offset-4 inline-block cursor-pointer md:hover:underline ${
					isRootWorks && 'text-[#4DAE9D]'
				}`}>Works</a
			>
			<div class="hidden md:flex items-center cursor-pointer  underline-offset-4 hover:underline">
				<GithubIcon />
				<a href="https://github.com/huseyincansoylu/portfolio" target="_blank" class="pl-1"
					>Source</a
				>
			</div>
		</div>
	</div>
</div>
