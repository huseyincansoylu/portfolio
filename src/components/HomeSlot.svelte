<script lang="ts">
	export let title: string;
</script>

<div class="mt-10">
	<h4
		class="text-xl font-semibold border-b-2 pb-2 border-[#6B46C1] dark:border-[#4DAE9D] inline-block"
	>
		{title}
	</h4>
	<slot />
</div>
