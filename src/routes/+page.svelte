<script>
	import ImageFigure from '$lib/ImageFigure.svelte';

	let caption = $state(
		'Skulls of a wildcat (top left), a housecat (top right), and a hybrid between the two (bottom center)'
	);
	let imageSrc = $state('catskull.png');
</script>

<h1>Fake Wikipedia Image Generator</h1>
<ImageFigure {caption} {imageSrc} />

<section>
	<div>
		<label for="caption">Caption (raw HTML)</label>
		<textarea bind:value={caption} id="caption" rows="7" cols="35"></textarea>
	</div>

	<div>
		<label for="imageUrl">Image URL</label>
		<input type="text" id="imageUrl" name="Image URL" bind:value={imageSrc} style="width: 400px;" />
	</div>
</section>

<footer>
	<p>created by <a href="https://www.justinliang.me/">justin</a></p>
	<a href="https://github.com/justinliang1020/fake-wikipedia">source code</a>
</footer>
