<script lang="ts">
    

    export let toggleCreacionArista: Function;
    export let creandoArista: boolean;

    function onClick() {
        toggleCreacionArista();
    }

</script>

<div class="mx-auto mt-4 text-white font-bold">
    {#if creandoArista}
        <button class="w-32 bg-red-700 hover:bg-red-500   px-4 py-2 rounded" on:click={onClick}>
            Cancelar
        </button>
    {:else}
        <button on:click={onClick} class="w-32 bg-blue-700 hover:bg-blue-500 py-2 px-4 rounded">
            Crear Arista
        </button>
    {/if}
</div>