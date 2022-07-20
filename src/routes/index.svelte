<script lang="ts">
	import GithubIcon from '../components/icons/GithubIcon.svelte';
	import ArrowRight from '../components/icons/ArrowRight.svelte';
	import StudyAndExperience from '../components/StudyAndExperience.svelte';
	import Instagram from '../components/icons/Instagram.svelte';
	import Linkedin from '../components/icons/Linkedin.svelte';
	import { educations, experience } from '../studyAndExperience';
</script>

<svelte:head>
	<title>Huseyin Can Soylu - Homepage</title>
</svelte:head>

<div class="mx-24">
	<div class="flex flex-col">
		<div class="mx-auto">
			<img src="/dev.png" alt="" />
		</div>

		<div class="w-full bg-[#313134] text-center py-4 rounded-lg">
			Hello, I'm a fullstack developer based in Turkey!
		</div>

		<div class="w-full flex mt-10">
			<div class="flex-1 ">
				<h1 class="text-4xl font-semibold">Huseyin Can Soylu</h1>
				<button class="px-4 py-2 rounded-md bg-[#4DAE9D] mt-6 font-semibold flex items-center font"
					>My portfolio <span class="ml-2 mt-1"><ArrowRight /></span>
				</button>
			</div>

			<div class="w-28">
				<img class="rounded-full border-2 border-gray-300" src="/canpg.jpg" alt="" />
			</div>
		</div>
	</div>
	<div class="mt-10">
		<h4 class="text-xl font-semibold border-b-2 pb-2 border-[#4DAE9D] inline-block">Bio</h4>
		<div class="mt-6">
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate placeat explicabo
				dolorum aut, necessitatibus aspernatur laboriosam ipsum non ullam libero exercitationem
				officia quasi repellat, earum ad est quia esse odio? Lorem ipsum dolor sit amet consectetur
				adipisicing elit. Cupiditate placeat explicabo dolorum aut, necessitatibus aspernatur
				laboriosam ipsum non ullam libero exercitationem officia quasi repellat, earum ad est quia
				esse odio?
			</p>
		</div>
	</div>
	<StudyAndExperience studyAndExperience={experience} title="Experience" />
	<StudyAndExperience studyAndExperience={educations} title="Education" />
	<div class="mt-10">
		<h4 class="text-xl font-semibold border-b-2 pb-2 border-[#4DAE9D] inline-block">I ♥</h4>
		<div class="mt-6">
			<p>Music, Playing guitar, Football, Ancient Cities, Travelling, Stand-up shows</p>
		</div>
	</div>

	<div class="mt-10">
		<h4 class="text-xl font-semibold border-b-2 pb-2 border-[#4DAE9D] inline-block">Social</h4>
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
	</div>
</div>
