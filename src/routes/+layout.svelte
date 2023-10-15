<script>
	import '../app.postcss';
	import './styles.css';
</script>

<div class="app">
	<header>
		<p class="title">はだかの王様</p>
	</header>
	<main>
		<slot />
	</main>

	<footer />
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		background-color: #fcfaf2;
	}

	header {
		display: flex;
		border-top: 1px solid #eaeaea;
		justify-content: left;
		align-items: center;
		padding-top: 12px;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 0 3%;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	.title {
		margin-left: 3.5%;
		font-size: small;
	}
	footer {
		padding: 6px 0;
	}

	@media (min-width: 480px) {
		footer {
			padding: 6px 0;
		}
	}
</style>
