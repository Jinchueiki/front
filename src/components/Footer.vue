<script setup> /* BALISE SCRIPT POUR JAVASCRIPT */
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template> <!-- BALISE TEMPLATE POUR HTML -->
<footer>
    <p> BDE éstiam Copyright 2022 </p>
</footer>
</template>

<style scoped> /* BALISE SCRIPT POUR CSS */
footer {
    background-color: #6231C6;
    text-align: center;
    width: 100%;
    margin: 0;
    padding: 0;
    color: #fff;
    font-size: 14px;
}
</style>