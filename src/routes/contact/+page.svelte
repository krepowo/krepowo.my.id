<script lang="ts">
	let showed = $state(false);

	function show_hide() {
		showed = true;
		setTimeout(() => {
			showed = false;
		}, 1000);
	}
	function copy(text: string) {
		navigator.clipboard.writeText(text);
		show_hide();
	}
</script>

<div class="mt-10 text-white backdrop-blur-sm bg-white/5 p-3 rounded-xl space-y-3">
	<h1 class="text-xl font-bold">Contact me</h1>
	<p>Feel free to send me a DM in Discord or send me an Email.</p>
	<ul>
		<li class="flex space-x-1 items-center">
			<p>- Discord: <button class="font-medium hover:bg-black/50 p-1 rounded-lg duration-200 hover:cursor-pointer" onclick={() => copy("@krepowo")}>@krepowo</button></p>
			<p class="bg-white/15 p-1 rounded-lg duration-200 transition-opacity ease-in-out text-sm {showed ? 'opacity-100' : 'opacity-0'}">Copied!</p>
		</li>
		<li class="items-center">
			<p>- Email: <a class="font-medium hover:bg-black/50 p-1 rounded-lg duration-200 hover:cursor-pointer" href="mailto:krepowo@gmail.com">krepowo@gmail.com</a></p>
		</li>
	</ul>

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
