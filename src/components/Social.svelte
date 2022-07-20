<script lang="ts">
	import GithubIcon from '../components/icons/GithubIcon.svelte';
	import Instagram from '../components/icons/Instagram.svelte';
	import Linkedin from '../components/icons/Linkedin.svelte';
	import HomeSlot from './HomeSlot.svelte';
</script>

<HomeSlot title="Social">
	<div class="grid grid-cols-3 gap-1 mt-6">
		<a
			href="https://github.com/huseyincansoylu"
			target="_blank"
			class="bg-[#313134] hover:bg-gray-200 py-3 hover:text-black text-center rounded-lg cursor-pointer flex items-center justify-center transition"
		>
			<span class="text-lg mr-2"><GithubIcon /></span>
			Github
		</a>
		<a
			href="https://www.linkedin.com/in/hcsoylu/"
			target="_blank"
			class="bg-[#313134] hover:bg-gray-200 py-3 hover:text-black text-center rounded-lg cursor-pointer flex items-center justify-center transition"
		>
			<span class="text-lg mr-2"><Linkedin /></span>
			Linkedin
		</a>
		<a
			href="https://www.instagram.com/hcsoylu/"
			target="_blank"
			class="bg-[#313134] hover:bg-gray-200 py-3 hover:text-black text-center rounded-lg cursor-pointer flex items-center justify-center transition"
		>
			<span class="text-lg mr-2"><Instagram /></span>
			Instagram
		</a>
	</div>
</HomeSlot>
