<script>
	import '../app.css';
	let { children } = $props();
</script>

<head>
	<title>KrepOwO</title>
</head>

<div id="background" class="min-h-screen w-screen bg-[url(bg.webp)] bg-cover fixed flex flex-col">
	<div id="isi" class="flex flex-col pt-10 pb-15 lg:pb-10 px-[1rem] md:px-[5rem] lg:px-[10rem] xl:px-[20rem] h-screen overflow-y-auto">
		<nav class="flex flex-row p-3 rounded-xl items-center justify-between backdrop-blur-sm bg-white/5">
			<a href="/" class="flex flex-row items-center space-x-3">
				<img src="/favicon.ico" alt="Logo" class="w-8" />
				<h1 class="text-2xl font-bold text-white">KrepOwO</h1>
			</a>
			<div class="md:flex lg:flex hidden space-x-10 text-white font-bold">
				<a href="/" class="flex flex-row items-center space-x-2">
					<img src="/home-white.svg" alt="Home" class="w-6" />
					<p>Home</p>
				</a>
				<a href="/projects" class="flex flex-row items-center space-x-2">
					<img src="/box-white.svg" alt="Projects" class="w-6" />
					<p>Projects</p>
				</a>
				<a href="/contact" class="flex flex-row items-center space-x-2">
					<img src="/mail-white.svg" alt="Contact" class="w-6" />
					<p>Contact</p>
				</a>
			</div>
		</nav>

		{@render children()}

		<div class="hidden lg:flex justify-center w-full py-3 left-0 text-white backdrop-blur-sm bg-white/5 rounded-xl text-sm mt-auto">
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

	<nav id="bottom-navbar" class="lg:hidden md:hidden fixed w-full bottom-0 py-3 left-0 text-white backdrop-blur-sm bg-white/5 items-center">
		<div class="flex space-x-10 text-white font-bold justify-center items-center px-5">
			<a href="/" class="flex flex-row items-center space-x-2">
				<img src="/home-white.svg" alt="Home" class="w-6" />
				<p>Home</p>
			</a>
			<a href="/projects" class="flex flex-row items-center space-x-2">
				<img src="/box-white.svg" alt="Projects" class="w-6" />
				<p>Projects</p>
			</a>
			<a href="/contact" class="flex flex-row items-center space-x-2">
				<img src="/mail-white.svg" alt="Contact" class="w-6" />
				<p>Contact</p>
			</a>
		</div>
	</nav>
</div>
