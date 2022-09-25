<script lang="ts">
	import Counter from '$lib/Counter.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="main">
	<h1>rip <span>afn</span></h1>
	<h2>
		A simple downloader for sites supported under youtube-dl
	</h2>

	<section class="hh">
		<button>Video</button>
		<button>Audio</button>
		<button>Playlist</button>
		<button>Thumbnail</button>
	</section>

	<form>
		<input
			placeholder="Video link" 
			type="text" 
			id="link" 
			name="l" 
			title="Paste link"
			required 
		>
		<br />
		<button></button>
	</form>

	<div class="info">
		<div class="image" style='background-image: url("https://i.ytimg.com/vi/YZDFAmaaa6E/hq720.jpg?sqp=-oaymwEcCNAFEJQDSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLBxl-x9SdLtea7R-qNrsPDsI3YLaA")'>
		</div>
		<div class="text">
			<h4>I've been trying to find this movie for 10 years</h4>
			<h2>Drew Gooden</h2>
			<h2>118 MB</h2>
		</div>
	</div>
</section>

<style>

	.main {
		display: flex;
		flex-direction: column;
		flex: 1;
	}

	h2 {
		margin-top: -0.25rem;
	}

	h4 {
		margin-bottom: 0.4rem;
	}

	span {
		color:var(--yellow);
	}
	
	form {
		display: flex;
		gap: 0.5rem;
		margin-bottom: 2.5rem;
	}

	button {
		font-family: var(--font-two);
		border: none;
		border: 1.5px solid var(--grey-three);
		background-color: transparent;
		color: var(--white);
		padding: 0.6rem 1.25rem;
		border-radius: 12px;
		font-size: 0.9rem;
		cursor: pointer;
	}

	.image {
		height: 9rem;
		background-size: cover;
		aspect-ratio: 16 / 9;
		border-radius: 12px;
	}

	.info {
		display:flex;
		gap: 3rem;
		background-color: var(--grey-one);
		border-radius: 12px;
	}

	.text {
		display: flex;
		flex-direction: column;
		justify-content: center;
		gap: 0.25rem;
	}


	input[type=text] {
		border: none;
		outline: none;

		border: 2px solid var(--grey-one);
		font-family: var(--font-two);
		width: 100%;
		height: 4rem;
		padding: 1rem;
		border-radius: 12px;
		color: var(--white);
		background-color: var(--grey-one);
		transition: all 0.2s var(--bezier-one);
	}

	input[type=text]:focus-within {
		border: 2px solid var(--yellow);
	}

	.hh {
		display:flex;
		gap: 0.5rem;
		margin-bottom: 1rem;
		margin-top: 2rem;
	}

</style>
