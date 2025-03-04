<script lang="ts">
    export let valor: string;
    $: tamanhoFonte = valor.length > 31 ? "pequena" : `s-${valor.length}`;
    console.log(valor.length);
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
        /* font-size: 1.7rem; */
        font-size: 4rem;
        justify-content: flex-end;
        align-items: center;
        background-color: aliceblue;
        border-top-right-radius: 5px;
        border-top-left-radius: 5px;
    }

    .s-17 {
        font-size: 3rem;
    }
    .s-18 {
        font-size: 3rem;
    }
    .s-19 {
        font-size: 3rem;
    }
    .s-20 {
        font-size: 3rem;
    }
    .s-21 {
        font-size: 3rem;
    }
    .s-22 {
        font-size: 2.5rem;
    }
    .s-23 {
        font-size: 2.5rem;
    }
    .s-24 {
        font-size: 2.5rem;
    }
    .s-25 {
        font-size: 2.5rem;
    }
    .s-26 {
        font-size: 2.4rem;
    }
    .s-27 {
        font-size: 2rem;
    }
    .s-28 {
        font-size: 2rem;
    }
    .s-29 {
        font-size: 2rem;
    }
    .s-30 {
        font-size: 2rem;
    }
    .s-31 {
        font-size: 2rem;
    }
    .pequena {
        font-size: 1.7rem;
    }
</style>
