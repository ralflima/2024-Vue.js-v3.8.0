<!-- SCRIPT -->
<script setup>

    // Importações
    import { onMounted, ref } from 'vue';

    // Vetor contendo as postagens
    let vetor = ref([]);

    // OnMounted
    onMounted(() => {
        fetch('https://jsonplaceholder.typicode.com/posts')
        .then(retorno => retorno.json())
        .then(retorno => vetor.value = retorno)
    });

</script>

<!-- HTML -->
<template>
    
    <h1>Requisições</h1>

    <table>
        <thead>
            <tr>
                <th>Código do usuário</th>
                <th>Código da postagem</th>
                <th>Título</th>
                <th>Comentário</th>
            </tr>
        </thead>

        <tbody>
            <tr v-for="v in vetor">
            <td>{{ v.userId }}</td>
            <td>{{ v.id }}</td>
            <td>{{ v.title }}</td>
            <td>{{ v.body }}</td>
        </tr>
        </tbody>
    </table>

</template>