<script>
	/* IMPORTS */
	import ImageRender from './ImageRender.svelte';
	import ButtonRender from './ButtonRender.svelte';
	import InputRender from './InputRender.svelte';

	/* VARIABLES */
	export let name;
</script>

<main>
	<h1>Welcome to {name} App!</h1>
	<h2>This is my first app with Svelte.</h2>

	<!-- <NOM_COMPONENT>VARIABLES = VALOR_VARIABLE</NOM_COMPONENT> -->

	<!-- COMPONENT QUE MOSTRA IMATGE -->
	<ImageRender></ImageRender>
	<!-- COMPONENT QUE CREA BOTONS -->
	<ButtonRender></ButtonRender>
	<!-- COMPONENT QUE CREA UN INPUT -->
	<InputRender></InputRender>
</main>


<!-- CANVIAR L'ESTIL DEL PARAGRAFS -->
<style>
	h2 {
		color: orangered;
		font-family: Verdana, Geneva, Tahoma, sans-serif;
		font-size: 1em;
	}
</style>