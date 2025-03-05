<script>
	let socials = [
		{
			name: 'Instagram',
			url: 'https://instagram.com/krepowo',
			icon: '/instagram.png'
		},
		{
			name: 'X / Twitter',
			url: 'https://twitter.com/Qwerty_Krep',
			icon: '/x.png'
		},
		{
			name: 'GitHub',
			url: 'https://github.com/krepowo',
			icon: '/github.png'
		},
		{
			name: 'YouTube',
			url: 'https://www.youtube.com/@krepowo',
			icon: '/youtube.png'
		}
	];
</script>

<div class="lg:space-y-8 space-y-5 mt-10">
	<div class="p-3 space-x-5 flex lg:flex-row flex-col items-center space-y-2 rounded-xl text-white font-mono backdrop-blur-sm bg-white/5">
		<div class="m-1 lg:pr-5">
			<img src="https://cdn.discordapp.com/avatars/620393180168323082/aae8b272bd5bf089c1e00b1c76a29b19.png?size=256" alt="Krep's avatar" class="size-15 lg:size-20 rounded-full" />
		</div>
		<div class="space-y-3">
			<h1 class="lg:text-3xl underline underline-offset-8 font-bold">Krep</h1>
			<p class="lg:text-lg text-sm">I like to gaming and make something with code.</p>
		</div>
	</div>

	<div class="p-3 rounded-xl text-white backdrop-blur-sm space-y-3 bg-white/5">
		<h1 class="text-white font-bold lg:text-xl">Connect with me</h1>
		<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4 w-full">
			{#each socials as social}
				<a href={social.url} target="_blank" rel="noopener noreferrer" class="flex flex-row text-white lg:text-lg space-x-2 justify-center items-center duration-200 hover:bg-black/50 p-2 rounded-xl">
					<img src={social.icon} alt={social.name} class="w-8" />
					<p>{social.name}</p>
				</a>
			{/each}
		</div>
		<div class="flex justify-center">
			<a href="https://discord.com/users/620393180168323082" class="flex items-center justify-center duration-200 hover:bg-black/50 p-2 rounded-xl" target="_blank">
				<img src="https://discord.c99.nl/widget/theme-4/620393180168323082.png" alt="My Discord Banner" />
			</a>
		</div>
	</div>

	<div class="lg:hidden w-full py-3 left-0 text-white backdrop-blur-sm bg-white/5 rounded-xl text-sm mt-auto">
		<div class="flex flex-col items-center">
			<div class="flex space-x-2">
				<a href="https://www.artstation.com/artwork/w8yDNV" class="underline" target="_blank">Background Source</a>
				<p>•</p>
				<a href="https://www.svgrepo.com/" class="underline" target="_blank">Icons</a>
			</div>
			<p>© 2025 KrepOwO. All Rights Reserved.</p>
		</div>
	</div>
</div>
