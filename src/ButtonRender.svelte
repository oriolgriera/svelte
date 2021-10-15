<script>
    /* VARIABLES */
    let count = 0;

    /* VARIABLES QUE DEPENEN D'ALTRES */
    $: resta = 10 - count;

    /* FUNCIONS */
    function incrementCount(){
        count += 1;
    }
    function resetCount(){
        count = 0;
    }

    /* CODI LLIURE */
    /* CODI QUE DEPEN DE LES VARIABLES */
    $: if (count > 10){
        count = 0
    }
</script>

<main>
	<!-- CREAR BOTÓ QUE EXECUTI FUNCIÓ -->
    <p>------------------------------------------------------</p>
    <h3>BUTTONS:</h3>
    <p>This is a button that counts the time you click:</p>
    <p>When at 10, it resets.</p>
    <p>{resta} Clicks to 10!</p>
	<button on:click={incrementCount}>
        Clicked {count} {count === 1 ? 'time' : 'times'}
    </button>
    <button on:click={resetCount}>
        Reset
    </button>
</main>