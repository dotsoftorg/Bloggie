<script>
	import logo from 'images/logo.png';
</script>

<style>
	figure {
		margin: 0 0 1em 0;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	@media (min-width: 480px) {
	}
</style>

<svelte:head>
	<title>Bloggie</title>
</svelte:head>

<figure>
	<img alt="Logo" src="{logo}">
	<figcaption>Some random text here</figcaption>
</figure>