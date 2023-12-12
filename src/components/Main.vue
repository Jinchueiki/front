<script setup> /* BALISE SCRIPT POUR JAVASCRIPT */
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
    <h1>PAGE PRINCIPALE</h1>
</template>

<style scoped>

</style>