<script setup>
const props = defineProps(['pessoas'])


</script>


<template>
    <tr>
        <td>{{ pessoas.nome }}</td>
        <td>{{ pessoas.cpf }}</td>
        <td>{{ pessoas.categoria }}</td>
        <td></td>
    </tr>
</template>