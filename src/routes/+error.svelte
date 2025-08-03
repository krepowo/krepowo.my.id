<script>
	import { page } from "$app/state";
</script>

<div class="flex flex-col items-center justify-center h-screen text-white">
	{#if page.status === 404}
		<h1 class="text-3xl font-bold">Page Not Found</h1>
		<p class="mt-2">The page you are looking for does not exist.</p>
	{:else if page.status === 500}
		<h1 class="text-3xl font-bold">Internal Server Error</h1>
		<p class="mt-2">Something went wrong on our end. Please try again later.</p>
	{:else}
		<h1 class="text-3xl font-bold">Error {page.status}</h1>
		<p class="mt-2">An unexpected error occurred. Please try again later.</p>
	{/if}
</div>
