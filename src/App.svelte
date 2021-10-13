<script>
	export let name;
</script>

<main>
	<h1>Welcome to {name} App!</h1>
	<p>This is my first app with Svelte.</p>
</main>

<style>
	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>