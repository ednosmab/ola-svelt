<script lang="ts">
    export let texto: string;
    export let triplo: boolean = false;
    export let duplo: boolean = false;
    export let operacao: boolean = false;
    export let destaque: boolean = false;
</script>

<button class="botao" class:triplo class:duplo class:operacao class:destaque>
    {texto}
</button>

<style>
    .botao {
        flex-basis: 25%;
        height: 35px;
        margin: 0;
        border: 1px solid var(--cor-fundo);
    }
    .triplo {
        flex-basis: 75%;
    }
    .duplo {
        flex-basis: 50%;
    }
    .operacao {
        background-color: orange;
        color: white;
    }
    .destaque {
        background-color: red;
        color: white;
    }
</style>
