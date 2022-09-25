<script lang="ts">
	import '../app.css';
</script>

<main class="wrapper">
	<slot />
	<!-- <span /> -->
</main>


<style>
	/* span {
		height: 25rem;
		width: 25rem;
		border: 3px solid var(--white);
		border-radius: 50%;
		position: absolute;
		z-index: -1;
		opacity: 0.25;
		transform: translate(-145%, -40%);
	} */
	main {
		display: flex;
		justify-content: center;
  		align-content: center;
	}
</style>
