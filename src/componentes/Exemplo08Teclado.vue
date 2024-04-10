<!-- SCRIPT -->
<script setup>

    // Função de mensagem
    function mensagem(){
        alert('Executando a função');
    }

</script>

<!-- HTML -->
<template>
    <input type="text" @keyup.r="mensagem">
</template>