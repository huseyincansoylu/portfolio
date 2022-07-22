<script lang="ts">
	export let title: string;
	import { page } from '$app/stores';
</script>

<div class={`${$page.routeId !== 'works' && 'mt-10'}`}>
	<h4
		class="text-xl font-semibold border-b-2 pb-2 border-gray-500 dark:border-[#4DAE9D] inline-block"
	>
		{title}
	</h4>
	<slot />
</div>
