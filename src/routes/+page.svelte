<script>
	import ImageFigure from '$lib/ImageFigure.svelte';

	let caption = $state(
		'Skulls of a wildcat (top left), a housecat (top right), and a hybrid between the two (bottom center)'
	);
</script>

<ImageFigure {caption} imageSrc="catskull.png" />

<form>
	<label for="caption">caption</label>
	<textarea bind:value={caption} id="caption" rows="7" cols="35"></textarea>
</form>
