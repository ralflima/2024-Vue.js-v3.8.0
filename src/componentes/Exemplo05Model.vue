<!-- SCRIPT -->
<script setup>
    
    // Importar o REF
    import { ref } from 'vue';

    // Variável
    let texto = ref('');

</script>

<!-- HTML -->
<template>
    <input type="text" v-model="texto">
    <p :class="teste ? 'ativo' : 'inativo'">{{ texto }}</p>
</template>