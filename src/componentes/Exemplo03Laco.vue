<!-- SCRIPT -->
<script setup>
    // Vetor
    let nomes = ['Alice', 'Bruna', 'Caio', 'Daniel', 'Ellen'];
</script>

<!-- HTML -->
<template>
    <ul>
        <li v-for="nome in nomes">{{ nome }}</li>
    </ul>
</template>