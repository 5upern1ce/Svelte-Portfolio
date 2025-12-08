<script>
	function badtothebone() {
		var audio = new Audio('bad-to-the-bone.mp3');
		audio.play();
	}
</script>

<svelte:head>
	<title>Graphic Design is My Passion</title>
</svelte:head>

<div class="w-full max-w-dvw overflow-x-hidden bg-linear-to-r from-yellow-300 to-green-500 pb-4" style="z-index: 1">
	<div class="flex w-3/4">
		<div class="animate-bounce md:pt-17">
			<img src="gojo-frolic.gif" alt="our glorious king frolicking" class="walkinggojo" />
		</div>
		<div class="w-full justify-items-center not-md:pt-30">
			<h1 class="comic-sans text-5xl font-extrabold">WELCOME TO MY EVIL LIER</h1>
		</div>
	</div>

	<div class="inline-flex w-full pt-6">
		<h2 class="comic-sans text-3xl font-bold">Hello, I am Ice and</h2>
		<img class="w-2/7 md:w-1/7" src="/graphic-design-is-my-passion.webp" alt="Graphic Design is My Passion" />
	</div>

	<h2 class="mt-3 ml-20 text-3xl font-bold md:ml-70">Here are 5 reasons you should hire me:</h2>

	<ol class="w-full list-decimal pt-10 md:pt-3">
		<li class="comic-sans w-75 justify-self-center rounded-3xl border-2 border-amber-600 bg-amber-400 text-5xl">1. I can center a div</li>

		<li class="comic-sans mr-10 w-1/2 justify-self-end rounded-3xl border-2 border-amber-600 bg-amber-400 text-5xl text-wrap md:w-1/3">
			3. My styles are consistent
		</li>

		<li
			class="comic-sans my-3 rounded-3xl border-2 border-amber-600 bg-amber-400 text-5xl sm:justify-self-start md:ml-60 md:inline-flex md:w-1/3 md:justify-self-auto"
		>
			C. My styles are <img src="/RAD.gif" alt="RAD" />
		</li>
		<br />

		<div class="pl-10">
			<li class="comic-sans my-3 inline-flex justify-self-center rounded-3xl border-2 border-amber-600 bg-amber-400 text-5xl md:w-1/3">
				I am bad to the bone (do NOT click on the skeleton)
				<button on:click={badtothebone} class="w-3/4 cursor-pointer md:h-full md:w-1/2">
					<img src="smilingskele.gif" alt="Rad smiling skeleton" class="rounded-3xl align-middle" />
				</button>
			</li>
		</div>
	</ol>

	<div class="my-3 flex justify-center">
		<a
			class="comic-sans w-1/2 cursor-pointer justify-self-center rounded-3xl border-2 border-amber-600 bg-amber-400 p-4 text-5xl md:w-1/3"
			id="codeworks"
			title="mycodeworks"
			href="broke"
		>
			My code always works too!
		</a>
	</div>

	<div class="py-4">
		<img src="walkingskele.gif" alt="Skele walking gif" class=" walkingskele" />
	</div>
</div>

<div class="flex w-full justify-center bg-amber-200 py-3">
	<a href="serious" title="serious" class="mb-4 w-3/4 rounded-lg border-2 bg-white p-3 text-center text-4xl font-semibold text-wrap md:min-w-1/3"
		>To my serious portfolio (99% less skeleton)</a
	>
</div>
