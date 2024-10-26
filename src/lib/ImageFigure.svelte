<script lang="ts">
	let { caption, imageSrc }: { caption: string; imageSrc: string } = $props();
</script>

<figure>
	<img src={imageSrc} alt="meow" />
	<figcaption>
		{@html caption}
	</figcaption>
</figure>

<style>
	figure {
		width: 229px;
		background-color: rgb(248, 249, 250);
		border: 1px solid #c8ccd1;
		border-bottom: 0;
		font-family: sans-serif;
		font-size: 16px;
		display: table;
	}

	img {
		max-width: calc(100% - (2 * 3px) - (2 * 1px));
		border: 1px solid #c8ccd1;
		margin: 3px;
	}

	figcaption {
		display: table-caption;
		caption-side: bottom;
		line-height: 1.4em;
		padding: 0 6px 6px 6px;
		border: 1px solid #c8ccd1;
		border-top: 0;
		background-color: #f8f9fa;
		font-size: 88%;
		background-image: url('https://en.wikipedia.org/w/resources/src/mediawiki.skinning/images/magnify-clip-ltr.svg?8330e');
		background-repeat: no-repeat;
		background-position: top right 5px;
	}
</style>
