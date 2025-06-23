<script>
	// @ts-nocheck

	export let imageLink = '';
	export let name = '';
	export let description = '';
	export let links = [];
</script>

<div id="project_card" class="w-full flex flex-col backdrop-blur-sm bg-white/5 p-3 rounded-xl text-white space-y-3">
	<h1 class="font-bold md:text-lg lg:text-xl">{name}</h1>
	<img src={imageLink} alt="Project's cover" class="w-full max-w-80 rounded-xl aspect-video object-cover mx-auto" />
	<p class="text-sm lg:text-base leading-5">{description}</p>

	<div class="flex space-x-3 mt-auto">
		{#each links as link}
			<a class="font-bold duration-200 p-1 hover:bg-gray-300/15 rounded-md" href={link.link} target="_blank">
				{link.name}
			</a>
		{/each}
	</div>
</div>
