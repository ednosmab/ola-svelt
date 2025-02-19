<script lang="ts">
    export let valor: string;
    $: tamanhoFonte = valor.length > 20 ? "pequena" : `s-${valor.length}`;
</script>

<div class={`tela ${tamanhoFonte}`}>
    <span>{valor}</span>
</div>

<style>
    .tela {
        display: flex;
        flex: 1;
        overflow: hidden;
        margin: 2px 1px;
        padding: 0 5px;
        font-size: 1.7rem;
        justify-content: flex-end;
        align-items: center;
        background-color: aliceblue;
        border-top-right-radius: 5px;
        border-top-left-radius: 5px;
    }

    .s-18 {
        font-size: 1.6rem;
    }
    .s-19 {
        font-size: 1.5rem;
    }
    .s-20 {
        font-size: 1.4rem;
    }

    .pequena {
        font-size: 1rem;
    }
</style>
