<script setup> /* BALISE SCRIPT POUR JAVASCRIPT */
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template> <!-- BALISE TEMPLATE POUR HTML -->
  <header>
        <div id="logo">
            <p><span>BDE </span>éstiam</p>
        </div>

        <ul id="menu">
            <li><a href="">Accueil</a></li>
            <li><a href="">Evenements</a></li>
            <li><a href="">Bons plans</a></li>
            <li><a href="">Membres</a></li>
            <li><a href="">Contact</a></li>
            <li><a href="">Boutique</a></li>
        </ul>

        <button id="account_btn">COMPTE</button>
    </header>
</template>

<style scoped> /* BALISE SCRIPT POUR CSS */
header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 20;
    background-color: #fff;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 8%;
    height: 50px;
    box-shadow: 0 0 10px 0 rgba(0,0,0,0.2);
}
#logo {
    color: #6231C6;
    font-size: 25px;
    font-weight: bold;
}
header .logo span {
    color: #000;
}
header button {
    background-color: #6231C6;
    cursor: pointer;
    color: #fff;
    padding: 5px 25px;
}
#menu {
    display: flex;
}
#menu li {
    list-style: none;
    margin: 0 15px;
}
#menu li a {
    font-size: 14px;
    color: #000;
    font-weight: 300;
    transition: 0.2s;
}
#menu li a:hover {
    color: #6231C6;
}
#account_btn {
  border-radius: 0;
}
</style>
