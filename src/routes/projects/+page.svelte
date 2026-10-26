<script>
	import ProjectCard from "$lib/ProjectCard.svelte";

	const projects = [
		{
			name: "osu2Discord",
			description: "Send osu! in-game chats to a Discord channel.",
			image: ["https://cdn.krepowo.my.id/file/osu2discord.png"],
			links: [
				{
					name: "GitHub",
					link: "https://github.com/krepowo/osu2discord"
				}
			]
		},
		{
			name: "IP Lookup Telegram Bot",
			description: "Lookup details about an IP address including location, ISP, and more. Trace, Track and Locate an IP address.",
			image: ["https://cdn.krepowo.my.id/file/iplookuptg.png"],
			links: [
				{
					name: "GitHub",
					link: "https://github.com/krepowo/IP-Lookup-TG"
				},
				{
					name: "Open in Telegram",
					link: "https://t.me/lookup_ip_bot"
				}
			]
		},
		{
			name: "Network Utils Discord Bot",
			description: "A Discord bot that provides network utilities such as DNS Lookup, Domain WHOIS, IP Lookup, and more.",
			image: ["https://cdn.krepowo.my.id/file/networkutils.png"],
			links: [
				{
					name: "Invite to Discord",
					link: "https://discordapp.com/oauth2/authorize?client_id=936446020441755708&permissions=1074120776&scope=bot"
				}
			]
		},
		{
			name: "OwOTools Discord Bot",
			description: "OwOTools is a Discord bot that have many utility tools like media downloader, search engine, and many more unique tools!",
			image: ["https://cdn.krepowo.my.id/file/owotools.gif"],
			links: [
				{
					name: "Invite to Discord",
					link: "https://discord.com/oauth2/authorize?client_id=1395956065484537866&permissions=262144&integration_type=0&scope=applications.commands+bot"
				},
				{
					name: "GitHub",
					link: "https://github.com/krepowo/OwOTools"
				}
			]
		},
		{
			name: "Freegame Notification Bot",
			description: "A discord bot that send a notification when there's a free game in Steam/Epic Games",
			image: ["https://cdn.krepowo.my.id/files/Discord_um8noT8k1P.png", "https://cdn.krepowo.my.id/files/Discord_4lFlUYVY8k.png"],
			links: []
		},
		{
			name: "Server Feedback Bot",
			description: "A discord bot for receiving server member's feedback.",
			image: ["https://cdn.krepowo.my.id/files/Discord_cJHzali350.png", "https://cdn.krepowo.my.id/files/Discord_Wb6bnQdBSV.png", "https://cdn.krepowo.my.id/files/Discord_YRCxAsTswe.png", "https://cdn.krepowo.my.id/files/Discord_3Bwd1jD6y8.png"],
			links: []
		},
		{
			name: "SquishVid",
			description: "Free, fast, and fully private video compression. No uploads, no accounts everything runs locally on your browsers.",
			image: ["https://cdn.krepowo.my.id/files/brave_7n0lC5wa3v.png"],
			links: [
				{
					name: "Visit",
					link: "https://squishvid.pages.dev"
				}
			]
		},
		{
			name: "osu! Beatmap Card",
			description: "Get an image card for your osu! Beatmap",
			image: ["https://cdn.krepowo.my.id/files/screenshot-2026-10-26-091639.png", "https://cdn.krepowo.my.id/files/beatmap-75-osucard%20%281%29.png", "https://cdn.krepowo.my.id/files/beatmap-75-poster.png", "https://cdn.krepowo.my.id/files/beatmap-75-glow.png"],
			links: [
				{
					name: "Visit",
					link: "https://cards.krepowo.my.id"
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

	<div class="flex flex-col items-center justify-center w-full mt-10">
		<a href="https://github.com/krepowo?tab=repositories" target="_blank" class="backdrop-blur-sm bg-white/5 hover:bg-white/20 text-white px-4 py-2 rounded-lg transition-colors duration-300">
			<p>More Projects...</p>
		</a>
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
