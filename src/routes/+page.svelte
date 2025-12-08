<script>
	function badtothebone() {
		var audio = new Audio('bad-to-the-bone.mp3');
		audio.play();
	}
</script>

<div class="bg-linear-to-r from-yellow-300 to-green-500 w-full pb-4 max-w-dvw overflow-x-hidden" style="z-index: 1">
	<div class="w-3/4 flex">
		<div class="animate-bounce pt-17">
			<img src="gojo-frolic.gif" alt="our glorious king frolicking" class="walkinggojo" />
		</div>
		<div class="w-full justify-items-center">
			<h1 class="comic-sans font-extrabold text-5xl">WELCOME TO MY EVIL LIER</h1>
		</div>
	</div>

	<div class="w-full inline-flex pt-6">
		<h2 class="comic-sans text-3xl font-bold">Hello, I am Ice and</h2>
		<img class="w-1/7" src="/graphic-design-is-my-passion.webp" alt="Graphic Design is My Passion" />
	</div>

	<h2 class="font-bold text-3xl mt-3 ml-60">Here are 5 reasons you should hire me:</h2>

	<ol class="w-full list-decimal pt-3">
		<li class="comic-sans text-5xl bg-amber-400 w-75 rounded-3xl border-2 border-amber-600 justify-self-center">1. I can center a div</li>

		<li class="comic-sans text-5xl bg-amber-400 w-1/3 rounded-3xl border-2 border-amber-600 justify-self-end">3. My styles are consistent</li>

		<li class="comic-sans text-5xl inline-flex ml-60 bg-amber-400 w-1/3 rounded-3xl border-2 border-amber-600">
			C. My styles are <img src="/RAD.gif" alt="RAD" />
		</li>
		<br />

		<div class="pl-10">
			<li class="comic-sans text-5xl inline-flex bg-amber-400 w-1/3 rounded-3xl border-2 border-amber-600 justify-self-center my-3">
				I am bad to the bone (do NOT click on the skeleton)
				<button on:click={badtothebone} class="w-1/2 h-full cursor-pointer">
					<img src="smilingskele.gif" alt="Rad smiling skeleton" class="rounded-3xl align-middle" />
				</button>
			</li>
		</div>
	</ol>

	<div class="my-3 flex justify-center">
		<a
			class="comic-sans text-5xl cursor-pointer bg-amber-400 w-1/3 rounded-3xl border-2 border-amber-600 justify-self-center p-4"
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

<div class="bg-amber-200 py-3 w-full flex justify-center">
	<a href="serious" title="serious" class="text-4xl p-3 font-semibold bg-white border-2 rounded-lg min-w-1/3 text-center text-wrap"
		>To my serious portfolio (99% less skeleton)</a
	>
</div>
