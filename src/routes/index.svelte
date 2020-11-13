<script>
	import successkid from 'images/successkid.jpg';
</script>

<style>
	h1, figure {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	figure {
		margin: 0 0 1em 0;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
			color: red;
		}
	}
</style>

<svelte:head>
	<title>Bloggie</title>
</svelte:head>

<h1>Bloggie</h1>

<figure>
	<img alt="Success Kid" src="{successkid}">
	<figcaption>Some random text here</figcaption>
</figure>