<!-- 
    Lifecycle: São ações que podem acontecer em três etapas de um componente:
    
    - Antes da criação;
    - Durante a criação;
    - Após a criação.
 -->









 
 <!-- SCRIPT -->
 <script setup>
    // Importações
    import { onMounted, ref } from 'vue';

    // Variável de texto
    let texto = ref('Hello World!');

    // Lifecycle onMounted
    onMounted(() => {
        setTimeout(() => {
            texto.value = 'Alterando texto!';   
        }, 3000);
    });
</script>

<!-- HTML -->
<template>
    <h1>{{ texto }}</h1>
</template>