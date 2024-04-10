 <!-- SCRIPT -->
 <script setup>

    // Obter Props
    const props = defineProps(['nome', 'idade', 'cidade', 'vetor', 'funcao']);

</script>

 <!-- HTML -->
 <template>
    <p>Nome: {{ nome }}</p>
    <p>Idade: {{ idade }}</p>
    <p>Cidade: {{ cidade }}</p>

    <ul>
        <li v-for="v of vetor">{{ v }}</li>
    </ul>

    <button @click="funcao">Clique aqui</button>
 </template>