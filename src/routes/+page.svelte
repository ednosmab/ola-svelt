<script>
    import Botao from "$lib/components/Botao.svelte";
    import Calculadora from "$lib/components/Calculadora.svelte";
</script>

<main>
    <Calculadora />
</main>

<style>
    :root {
        font-size: 62.5%;
    }
    :global(html, body) {
        margin: 0;
        padding: 0;
    }
    :global(*) {
        box-sizing: border-box;
    }
    :global(body) {
        background-color: black;
    }
    main {
        margin: 0;
        padding: 0;
    }
    main {
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>
