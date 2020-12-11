<template>
    <div id="clientes">
        <h2 id="titulo">Nome: {{cliente.nome}}</h2>
        <p>Email: {{cliente.email}}</p>
        <span v-show="show" >Idade: {{cliente.idade}}</span>
    </div>

</template>

<script>

// import Produtos from './Produtos';

export default {
    data() {
        return {
        }
    },
    props: {

        cliente: Object,
        show: Boolean
    },
    components: {
        // Produtos
    }
}

</script>

<style>
    #clientes{
       background: #D3D3D3;
       width: 30%;
       padding: 3px;
       margin-bottom: 4px;
    }
    #titulo{
        color: red;
    }
</style>