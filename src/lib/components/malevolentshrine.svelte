<script lang="ts">
	import { onMount } from 'svelte';

	let canvas: HTMLCanvasElement;
	let ctx: CanvasRenderingContext2D;

	function windowsize() {
		ctx.canvas.width = window.innerWidth - 20;
		ctx.canvas.height = window.innerHeight - 20;
	}

	onMount(() => {
		const context = canvas.getContext('2d');
		if (context) {
			console.log(context);
			ctx = context;
		}

		windowsize();
		window.addEventListener('resize', windowsize);

		main();
	});
	function getRandom(max: number) {
		return Math.floor(Math.random() * max);
	}

	function setLine(startx: any, starty: number, endx: any, endy: number, speed: number, backward: boolean, lineNumber = 0, lines = 10, widthln = 10) {
		let currentx = startx;
		let currenty = starty;

		drawLine(startx, starty, endx, endy, speed, currentx, currenty, backward, lineNumber, lines, widthln);
	}

	function drawLine(
		startx: number,
		starty: number,
		endx: number,
		endy: number,
		speed: number,
		currentx: number,
		currenty: number,
		backward: boolean,
		lineNumber = 0,
		lines = 10,
		widthln: number
	) {
		console.log(currentx);
		console.log(currenty);
		// ctx.clearRect(0, 0, canvas.clientWidth, canvas.clientHeight);
		ctx.lineWidth = widthln + 15;
		ctx.strokeStyle = 'black';
		ctx.fillStyle = 'white';
		ctx.beginPath();
		ctx.moveTo(startx, starty);
		ctx.lineTo(currentx, currenty);
		ctx.fill();
		ctx.stroke();
		ctx.lineWidth -= 5;
		ctx.strokeStyle = 'white';
		ctx.stroke();
		ctx.lineWidth -= 10;
		ctx.strokeStyle = 'red';
		ctx.stroke();

		if (backward != true) {
			if (currentx < endx) {
				requestAnimationFrame(() =>
					drawLine(
						startx,
						starty,
						endx,
						endy,
						speed,
						currentx + (endx - startx) * speed,
						currenty + (endy - starty) * speed,
						backward,
						lineNumber,
						lines,
						widthln
					)
				);
			} else {
				ctx.clearRect(0, 0, canvas.clientWidth, canvas.clientHeight);
				if (lineNumber < lines) {
					initline((lineNumber += 1), lines);
				}
				return;
			}
		} else {
			if (currentx >= endx) {
				requestAnimationFrame(() =>
					drawLine(
						startx,
						starty,
						endx,
						endy,
						speed,
						currentx + (endx - startx) * speed,
						currenty + (endy - starty) * speed,
						backward,
						lineNumber,
						lines,
						widthln
					)
				);
			} else {
				ctx.clearRect(0, 0, canvas.clientWidth, canvas.clientHeight);
				if (lineNumber < lines) {
					initline((lineNumber += 1), lines);
				}
				return;
			}
		}
	}

	function initline(lineNumber = 0, lines = 10) {
		console.log('initline ' + lineNumber);
		let starty = getRandom(ctx.canvas.height);
		let endy = getRandom(ctx.canvas.height);
		let speed = 0.05;
		let backward = false;
		let widthln = getRandom(4);
		console.log('Lets done');
		let startx, endx;
		if (getRandom(2) === 0) {
			startx = 0;
			endx = ctx.canvas.width;
		} else {
			startx = ctx.canvas.width;
			endx = 0;
			backward = true;
		}
		console.log('if statement done ');
		setLine(startx, starty, endx, endy, speed, backward, lineNumber, lines, widthln);
	}

	function main() {
		initline(0, 100);
		initline(0, 100);
		initline(0, 100);
	}

	// main();
</script>

<canvas style="background-color: transparent; z-index:1000; position: absolute " bind:this={canvas}> </canvas>
