<!-- SCRIPT -->
<script setup>

    // Função para validar o formulário
    function validaFormulario(event){
        alert('Formulário enviado!');

        event.preventDefault();
    }

</script>

<!-- HTML -->
<template>
    <form action="http://www.ralflima.com" @submit="validaFormulario">
        <input type="submit" value="Enviar formulário">
    </form>
</template>