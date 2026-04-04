<script>
	// @ts-nocheck

	export let imageLink = []; // now supports string[]
	export let name = "";
	export let description = "";
	export let links = [];

	let isGalleryOpen = false;
	let currentIndex = 0;

	$: images = Array.isArray(imageLink) ? imageLink.filter(Boolean) : [imageLink].filter(Boolean);
	$: if (currentIndex >= images.length) currentIndex = 0;

	function openGallery(index = 0) {
		currentIndex = index;
		isGalleryOpen = true;
	}

	function closeGallery() {
		isGalleryOpen = false;
	}

	function prevImage() {
		if (images.length < 2) return;
		currentIndex = (currentIndex - 1 + images.length) % images.length;
	}

	function nextImage() {
		if (images.length < 2) return;
		currentIndex = (currentIndex + 1) % images.length;
	}
</script>

<div id="project_card" class="w-full flex flex-col backdrop-blur-sm bg-white/5 p-3 rounded-xl text-white space-y-3">
	<h1 class="font-bold md:text-lg lg:text-xl">{name}</h1>

	{#if images.length > 0}
		<button type="button" class="mx-auto w-full max-w-80" on:click={() => openGallery(0)}>
			<img src={images[0]} alt="Project's cover" class="w-full rounded-xl aspect-video object-contain object-center bg-black/10 hover:bg-black/50 duration-200 hover:cursor-pointer" />
		</button>
	{/if}

	<p class="text-sm lg:text-base leading-5">{description}</p>

	{#if links.length > 0}
		<div class="flex space-x-3 mt-auto">
			{#each links as link}
				<a class="font-bold duration-200 p-1 hover:bg-gray-300/15 rounded-md" href={link.link} target="_blank" rel="noopener noreferrer">
					{link.name}
				</a>
			{/each}
		</div>
	{/if}
</div>

{#if isGalleryOpen && images.length > 0}
	<div class="fixed inset-0 z-50 bg-black/90 flex items-center justify-center p-4">
		<button type="button" class="absolute inset-0" aria-label="Close gallery" on:click={closeGallery}></button>

		<div class="relative w-full max-w-5xl z-10">
			<button type="button" class="absolute -top-10 right-0 text-white text-3xl leading-none hover:cursor-pointer" on:click={closeGallery} aria-label="Close gallery">×</button>

			<div class="relative flex items-center justify-center">
				{#if images.length > 1}
					<button type="button" class="absolute left-2 md:left-4 text-white text-3xl leading-none bg-black/40 hover:bg-black/60 hover:cursor-pointer rounded-full w-10 h-10 flex items-center justify-center text-center size-6" on:click={prevImage} aria-label="Previous image">
						<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="size-6">
							<path fill-rule="evenodd" d="M7.72 12.53a.75.75 0 0 1 0-1.06l7.5-7.5a.75.75 0 1 1 1.06 1.06L9.31 12l6.97 6.97a.75.75 0 1 1-1.06 1.06l-7.5-7.5Z" clip-rule="evenodd" />
						</svg>
					</button>
				{/if}

				<img src={images[currentIndex]} alt={`Gallery image ${currentIndex + 1}`} class="w-full max-h-[75vh] object-contain object-center rounded-lg" />

				{#if images.length > 1}
					<button type="button" class="absolute right-2 md:right-4 text-white text-3xl leading-none bg-black/40 hover:bg-black/60 hover:cursor-pointer rounded-full w-10 h-10 flex items-center justify-center text-center size-6" on:click={nextImage} aria-label="Next image">
						<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="size-6">
							<path fill-rule="evenodd" d="M16.28 11.47a.75.75 0 0 1 0 1.06l-7.5 7.5a.75.75 0 0 1-1.06-1.06L14.69 12 7.72 5.03a.75.75 0 0 1 1.06-1.06l7.5 7.5Z" clip-rule="evenodd" />
						</svg>
					</button>
				{/if}
			</div>

			{#if images.length > 1}
				<div class="mt-4 flex gap-2 overflow-x-auto justify-center">
					{#each images as img, i}
						<button type="button" class={`rounded-md overflow-hidden border-2 ${i === currentIndex ? "border-white" : "border-transparent"}`} on:click={() => (currentIndex = i)} aria-label={`Open image ${i + 1}`}>
							<img src={img} alt={`Thumbnail ${i + 1}`} class="w-16 h-10 object-cover" />
						</button>
					{/each}
				</div>
			{/if}
		</div>
	</div>
{/if}
