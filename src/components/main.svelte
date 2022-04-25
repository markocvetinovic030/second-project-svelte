<script>
	let jupiter = '../src/image/jupiter.jpg';
	let mars = '../src/image/mars.jpg';
	let merkur = '../src/image/merkur.jpg';
	let neptun = '../src/image/neptun.jpg';
	let saturn = '../src/image/jupiter.jpg';
	let uran = '../src/image/jupiter.jpg';
	let venera = '../src/image/venera.png';
	let zemlja = '../src/image/zemlja.jpg';
	import Hidden from './Hidden.svelte';

	let shown;
	let show;
</script>

<div class="bg-black p-40 ">
	<div class="flex justify-between w-8/12 m-auto">
		<div>
			<img class=" rounded-full" src={merkur} alt="merkur" />
			<p class=" text-white font-extralight text-center text-2xl pt-10 ">MERCURY</p>

			<div>
				<Hidden bind:shown bind:show>
					<p
						class="text-white w-48 border-b-2 border-t-2 m-auto p-6 mt-10 text-center duration-300"
					>
						Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eget placerat nibh,
						eget venenatis quam.
					</p>
				</Hidden>
			</div>
		</div>

		<div>
			<img class=" rounded-full" src={venera} alt="venera" />
			<p class="text-white font-extralight text-center text-2xl pt-10 ">VENUS</p>
			<button class="bg-white w-16 h-16 rounded-full mt-10 block m-auto hover:animate-bounce"
				><img class="w-8 m-auto" src="../src/image/download.png" alt="down" /></button
			>
		</div>
		<div>
			<img class="rounded-full" src={zemlja} alt="zemlja" />
			<p class="text-white font-extralight text-center text-2xl pt-10 ">EARTH</p>
			<button class="bg-white w-16 h-16 rounded-full mt-10 block m-auto hover:animate-bounce"
				><img class="w-8 m-auto" src="../src/image/download.png" alt="down" /></button
			>
		</div>
		<div>
			<img class=" rounded-full " src={mars} alt="mars" />
			<p class="text-white font-extralight text-center text-2xl pt-10 ">MARS</p>
			<button class="bg-white w-16 h-16 rounded-full mt-10 block m-auto hover:animate-bounce"
				><img class="w-8 m-auto" src="../src/image/download.png" alt="down" /></button
			>
		</div>
	</div>
</div>
