<script lang="ts">
	import StudyAndExperience from '../components/StudyAndExperience.svelte';
	import Welcome from '../components/Welcome.svelte';
	import { educations, experience } from '../data';
	import Social from '../components/Social.svelte';
	import Hobbies from '../components/Hobbies.svelte';
	import MyPortfolio from '../components/MyPortfolio.svelte';
	import Bio from '../components/Bio.svelte';
	import HomeSlot from '../components/HomeSlot.svelte';
</script>

<svelte:head>
	<title>Huseyin Can Soylu - Homepage</title>
</svelte:head>

<Welcome />
<MyPortfolio />
<Bio />
<HomeSlot title="Experiences">
	<StudyAndExperience studyAndExperience={experience} />
</HomeSlot>
<HomeSlot title="Education">
	<StudyAndExperience studyAndExperience={educations} />
</HomeSlot>
<Hobbies />
<Social />
