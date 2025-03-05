<script>
	import ProjectCard from '$lib/ProjectCard.svelte';

	const projects = [
		{
			name: 'osu2Discord',
			description: 'Send osu! in-game chats to a Discord channel.',
			image: 'https://cdn.krepowo.my.id/file/osu2discord.png',
			links: [
				{
					name: 'GitHub',
					link: 'https://github.com/krepowo/osu2discord'
				}
			]
		},
		{
			name: 'IP Lookup Telegram Bot',
			description: 'Lookup details about an IP address including location, ISP, and more. Trace, Track and Locate an IP address.',
			image: 'https://cdn.krepowo.my.id/file/iplookuptg.png',
			links: [
				{
					name: 'GitHub',
					link: 'https://github.com/krepowo/IP-Lookup-TG'
				},
				{
					name: 'Open in Telegram',
					link: 'https://t.me/lookup_ip_bot'
				}
			]
		},
		{
			name: 'Network Utils Discord Bot',
			description: 'A Discord bot that provides network utilities such as DNS Lookup, Domain WHOIS, IP Lookup, and more.',
			image: 'https://cdn.krepowo.my.id/file/networkutils.png',
			links: [
				{
					name: 'Invite to Discord',
					link: 'https://discordapp.com/oauth2/authorize?client_id=936446020441755708&permissions=1074120776&scope=bot'
				}
			]
		}
	];
</script>

<div class="space-y-5">
	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 w-full mt-10">
		{#each projects as project}
			<ProjectCard imageLink={project.image} name={project.name} description={project.description} links={project.links} />
		{/each}
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
