<script setup> /* BALISE SCRIPT POUR JAVASCRIPT */
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template> <!-- BALISE TEMPLATE POUR HTML -->
<footer>
    <div id="pages">
        <a href="./components/App.vue">Accueil</a>
        <a href="./components/Event.vue">Evenements</a>
        <a href="./components/Offers.vue">Bons plans</a>
        <a href="./components/Members.vue">Membres</a>
        <a href="./components/Contact.vue">Contact</a>
        <a href="./components/Shop.vue">Boutique</a>
    </div>
    <div id="contacts">Contacts
        Address : 29 avenue Leclerc
        Number : 04 28 29 25 75
        City : 69007 Lyon
        Mail : bde.estiam.lyon7@gmail.com
    </div>
    <div id="reseaux">Réseaux
        <a href="https://www.instagram.com/bde.estiam_lyon">Instagram</a>
        <a href="https://discord.com/invite/wwKDpn7r">Discord</a>
        <a href="https://www.facebook.com/profile.php/?id=100068550985078&name=xhp_nt__fb__action__open_user&locale=fr_FR">Facebook</a>
    </div>

</footer>
</template>

<style scoped> /* BALISE SCRIPT POUR CSS */
footer {
    display: inline-block;
    background-color: #6231C6;
    text-align: center;
    width: 100%;
    margin: 0;
    padding: 5px;
    color: #fff;
    font-size: 20px;
    bottom: 0;
}

#pages {
    width: 30%;
    display: inline-block;
}

#contacts {
    width: 30%;
    display: inline-block;
}

#reseaux {
    width: 30%;
    display: inline-block;
}
</style>