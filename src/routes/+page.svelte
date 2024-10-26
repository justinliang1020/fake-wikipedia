<script>
	import ImageFigure from '$lib/ImageFigure.svelte';

	let caption = $state(
		'Skulls of a wildcat (top left), a housecat (top right), and a hybrid between the two (bottom center)'
	);
	let imageSrc = $state('catskull.png');
</script>

<ImageFigure {caption} {imageSrc} />
<label for="caption">caption</label>
<textarea bind:value={caption} id="caption" rows="7" cols="35"></textarea>

<br />

<label for="imageUrl">Image URL</label>
<input type="text" id="imageUrl" name="Image URL" bind:value={imageSrc} />
