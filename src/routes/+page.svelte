<script>
	const socials = [
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
		},
		{
			name: 'Steam',
			url: 'https://steamcommunity.com/id/krepowo',
			icon: '/steam.png'
		}
	];

	const progLanguage = [
		{
			name: 'JavaScript',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg',
			url: 'https://developer.mozilla.org/en-US/docs/Web/JavaScript'
		},
		{
			name: 'Python',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg',
			url: 'https://www.python.org/'
		},
		{
			name: 'TypeScript',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg',
			url: 'https://www.typescriptlang.org/'
		}
	];

	const frontEnd = [
		{
			name: 'Svelte',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/svelte/svelte-original.svg',
			url: 'https://svelte.dev/'
		},
		{
			name: 'React',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg',
			url: 'https://react.dev/'
		},
		{
			name: 'TailwindCSS',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg',
			url: 'https://tailwindcss.com/'
		},
		{
			name: 'NextJS',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nextjs/nextjs-original.svg',
			url: 'https://nextjs.org/'
		},
		{
			name: 'HTML',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg',
			url: 'https://developer.mozilla.org/en-US/docs/Web/HTML'
		},
		{
			name: 'CSS',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg',
			url: 'https://developer.mozilla.org/en-US/docs/Web/CSS'
		}
	];

	const backEnd = [
		{
			name: 'Node.js',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original.svg',
			url: 'https://nodejs.org/'
		},
		{
			name: 'Express',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/express/express-original.svg',
			url: 'https://expressjs.com/'
		},
		{
			name: 'Prisma',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/prisma/prisma-original.svg',
			url: 'https://www.prisma.io/'
		},
		{
			name: 'Drizzle',
			icon: '/drizzle.png',
			url: 'https://orm.drizzle.team/'
		},
		{
			name: 'MySQL',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg',
			url: 'https://www.mysql.com/'
		},
		{
			name: 'PostgreSQL',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg',
			url: 'https://www.postgresql.org/'
		},
		{
			name: 'MongoDB',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg',
			url: 'https://www.mongodb.com/'
		}
	];
	const tools = [
		{
			name: 'Git',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg',
			url: 'https://git-scm.com/'
		},
		{
			name: 'Docker',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg',
			url: 'https://www.docker.com/'
		},
		{
			name: 'Vercel',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vercel/vercel-original.svg',
			url: 'https://vercel.com/'
		},
		{
			name: 'Netlify',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/netlify/netlify-original.svg',
			url: 'https://www.netlify.com/'
		},
		{
			name: 'VSCode',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vscode/vscode-original.svg',
			url: 'https://code.visualstudio.com/'
		},
		{
			name: 'Ubuntu',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/ubuntu/ubuntu-original.svg',
			url: 'https://ubuntu.com/'
		},
		{
			name: 'Windows',
			icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/windows8/windows8-original.svg',
			url: 'https://www.microsoft.com/windows/'
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

		<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-4 w-full duration-200 hover:bg-black/10 rounded-xl p-1">
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

	<div class="p-3 rounded-xl text-white backdrop-blur-sm space-y-3 bg-white/5">
		<h1 class="text-white font-bold lg:text-xl">Language and Tools</h1>

		<div class="w-full flex lg:flex-col flex-col justify-center space-y-3 lg:space-y-3 p-3">
			<div class="flex flex-col">
				<h2 class="text-white font-bold lg:text-lg">Languages</h2>
				<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 xl:grid-cols-6 gap-2 w-full duration-200 hover:bg-black/10 rounded-xl p-1">
					{#each progLanguage as lang}
						<a href={lang.url} target="_blank" rel="noopener noreferrer" class="flex flex-row text-white lg:text-lg space-x-2 duration-200 hover:bg-black/50 p-2 rounded-xl">
							<img src={lang.icon} alt={lang.name} class="w-8" />
							<p>{lang.name}</p>
						</a>
					{/each}
				</div>
			</div>
			<div class="flex flex-col">
				<h2 class="text-white font-bold lg:text-lg">Frontend</h2>
				<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 xl:grid-cols-6 gap-2 w-full duration-200 hover:bg-black/10 rounded-xl p-1">
					{#each frontEnd as fe}
						<a href={fe.url} target="_blank" rel="noopener noreferrer" class="flex flex-row text-white lg:text-lg space-x-2 duration-200 hover:bg-black/50 p-2 rounded-xl">
							<img src={fe.icon} alt={fe.name} class="w-8" />
							<p>{fe.name}</p>
						</a>
					{/each}
				</div>
			</div>
			<div class="flex flex-col">
				<h2 class="text-white font-bold lg:text-lg">Backend</h2>
				<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 xl:grid-cols-6 gap-2 w-full duration-200 hover:bg-black/10 rounded-xl p-1">
					{#each backEnd as be}
						<a href={be.url} target="_blank" rel="noopener noreferrer" class="flex flex-row text-white lg:text-lg space-x-2 duration-200 hover:bg-black/50 p-2 rounded-xl">
							<img src={be.icon} alt={be.name} class="w-8" />
							<p>{be.name}</p>
						</a>
					{/each}
				</div>
			</div>
			<div class="flex flex-col">
				<h2 class="text-white font-bold lg:text-lg">Tools</h2>
				<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 xl:grid-cols-6 gap-2 w-full duration-200 hover:bg-black/10 rounded-xl p-1">
					{#each tools as tool}
						<a href={tool.url} target="_blank" rel="noopener noreferrer" class="flex flex-row text-white lg:text-lg space-x-2 duration-200 hover:bg-black/50 p-2 rounded-xl">
							<img src={tool.icon} alt={tool.name} class="w-8" />
							<p>{tool.name}</p>
						</a>
					{/each}
				</div>
			</div>
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
