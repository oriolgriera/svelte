<script>
    /* VARIABLES */
    export let name = "";
    export let num = 0;
</script>

<main>
	<!-- CREAR UN INPUT -->
    <p>------------------------------------------------------</p>
    <p>Introduce your name:</p>
    <!-- EL BIND VINCULA EL VALOR DEL INPUT AMB LA VARIABLE -->
	<input bind:value={name}>
    <p>Hello {name}!</p>
    <p>Choose a number:</p>
    <!-- ES POT ESPECIFICAR QUE EL INPUT ES D'UN TIPUS CONCRET -->
    <input type=number bind:value={num} min=0 max=10>
	<input type=range bind:value={num} min=0 max=10>
    
    <p>------------------------------------------------------</p>
</main>