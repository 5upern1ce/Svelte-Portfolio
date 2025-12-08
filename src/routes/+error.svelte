<script lang="ts">
	import { page } from '$app/state';
	console.log('bro get out of the console');
	console.log("also play Zelda: Ocarina of Time shit's peak");
</script>

<div class="grid w-full justify-items-center">
	<h1 class="col-span-3 flex justify-center pt-6 text-5xl font-bold">{page.status}</h1>
	<h2 class=" col-span-3 flex justify-center pb-4 text-2xl font-bold">{page.error.message}</h2>
	<a
		class=" col-span-3 h-full w-1/2 max-w-[400px] border-2 bg-purple-300 justify-center rounded-md object-cover px-4 py-2 pt-3 text-center font-bold text-wrap"
		href="/"
	>
		Return to the home page
		<img src="smilingskele.gif" alt="Rad smiling skeleton" class="rounded-3xl w-1/4 aspect-square justify-self-center" />
	</a>
</div>
