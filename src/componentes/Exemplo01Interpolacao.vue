<!-- SCRIPT -->
<script setup>

  // Variáveis
  let nome = 'Rebeca';
  let idade = 32;
  let numero1 = 20;
  let numero2 = 10;
  
</script>

<!-- HTML -->
<template>
  <p>{{ 'Olá ' + nome + ' você tem ' + idade + ' anos.' }}</p>
  <p>{{ numero1+numero2 }}</p>
</template>