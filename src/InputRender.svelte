<script>
    /* VARIABLES */
    export let name = "";
    export let num = 0;
    export let check = false;
</script>

<main>
	<!-- CREAR UN INPUT -->
    <p>------------------------------------------------------</p>
    <h3>INPUTS:</h3>
    <p>Introduce your name:</p>
    <!-- EL BIND VINCULA EL VALOR DEL INPUT AMB LA VARIABLE -->
	<input bind:value={name}>
    <p>Hello {name}!</p>
    <p>Choose a number:</p>
    <!-- ES POT ESPECIFICAR QUE EL INPUT ES D'UN TIPUS CONCRET -->
    <!-- TIPUS NÚMERO -->
    <input type=number bind:value={num} min=0 max=10>
    <!-- TIPUS NÚMERO AMB RANG -->
	<input type=range bind:value={num} min=0 max=10>
    <!-- TIPUS CHECKBOX -->
    <label>
        <br>
        <input type=checkbox bind:checked={check}>
        Check?
    </label>
    {#if check}
	<p>It is checked!</p>
    {:else}
	<p>It is NOT checked!</p>
    {/if}
    
    

    <p>------------------------------------------------------</p>
</main>