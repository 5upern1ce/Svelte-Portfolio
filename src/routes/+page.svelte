<script>
	function badtothebone() {
		var audio = new Audio('bad-to-the-bone.mp3');
		audio.play();
	}
</script>

<svelte:head>
	<title>Graphic Design is My Passion</title>
</svelte:head>

<div class="relative z-0 h-full w-full max-w-dvw overflow-x-hidden bg-linear-to-r from-yellow-300 to-green-500 pb-4">
	<img src="link-fall.gif" alt="Link Falling" class="fallinglink z-10 not-md:invisible" />
	<div class="flex w-3/4">
		<div class="w-full animate-bounce pt-17">
			<img src="gojo-frolic.gif" alt="our glorious king frolicking" class="walkinggojo sticky aspect-square md:w-1/6" />
		</div>
		<div class="w-full justify-items-center pt-6">
			<h1 class="comic-sans text-center text-5xl font-extrabold">WELCOME TO MY EVIL LAIR</h1>
			<div class="absolute justify-items-end not-md:invisible">
				<img src="gojo-tweak.gif" alt="Gojo Tweaking" class=" z-20 animate-spin rounded-full p-10 md:absolute" />
				<img src="fire.gif" alt="fire" class="sticky z-10 flex w-1/2" />
			</div>
		</div>
	</div>

	<div class="inline-flex w-3/4 gap-1 pt-6">
		<h2 class="comic-sans text-end text-3xl font-bold text-nowrap">Hello, I am Ice and</h2>
		<img class="w-2/7 md:w-1/7" src="/graphic-design-is-my-passion.webp" alt="Graphic Design is My Passion" />
	</div>

	<h2 class="mt-3 ml-20 text-3xl font-bold md:ml-70">Here are 5 reasons you should hire me:</h2>

	<ol class="w-full list-decimal pt-10 md:pt-3">
		<div class="w-3/4">
			<li class="comic-sans justify-self-center rounded-3xl border-2 border-amber-600 bg-amber-400 text-5xl not-md:w-1/2">I can center a div</li>
		</div>
		<li class="comic-sans mr-10 w-1/2 justify-self-end rounded-3xl border-2 border-amber-600 bg-amber-400 text-5xl text-wrap md:w-1/3">
			3. My styles are consistent
		</li>

		<li
			class="comic-sans my-3 rounded-3xl border-2 border-amber-600 bg-amber-400 text-5xl sm:justify-self-start md:ml-60 md:max-w-1/5 md:justify-self-auto"
		>
			C. My styles are <img src="/RAD.gif" alt="RAD" class="" />
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
			class="comic-sans w-1/2 cursor-pointer justify-self-center rounded-3xl border-2 border-amber-600 bg-amber-400 p-4 text-center text-5xl md:w-1/3"
			id="codeworks"
			title="mycodeworks"
			href="broke"
		>
			My code always works too!
		</a>
	</div>

	<div
		class="comic-sans my-3 flex w-full justify-center justify-self-center rounded-3xl border-2 border-amber-600 bg-amber-400 p-4 text-center text-5xl md:w-1/3"
	>
		And I never over complicate my pages!
	</div>

	<div class="justify-self-center md:w-1/7">
		<a href="darkfantasy" class="justify-center">
			<h1 class="comic-sans text-2xl font-semibold">Come on an Adventure</h1>
			<img src="darkfantasy/knightslumpedover.jpg" alt="Dark Fantasy Knight" class="w-full rounded-lg" />
		</a>
	</div>

	<div class="py-3">
		<img src="walkingskele.gif" alt="Skele walking gif" class=" walkingskele" />
	</div>
</div>

<div class="flex w-full justify-center bg-amber-200 py-3">
	<a href="serious" title="serious" class="mb-4 w-3/4 rounded-lg border-2 bg-white p-3 text-center text-4xl font-semibold text-wrap md:min-w-1/3"
		>To my serious portfolio (99% less skeleton)</a
	>
</div>
