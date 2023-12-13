<script setup>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

import Shop from './components/Shop.vue';
import Offers from './components/Offers.vue';
import Members from './components/Members.vue';
import Main from './components/Main.vue';
import Event from './components/Event.vue';
import Contact from './components/Contact.vue';

</script>

<template>
  <div>
    <Header />
    <component :is="currentComponent" @switch-component="switchComponent" />
    <Footer />
  </div>
</template>

<style scoped>

</style>

<script>

  const data = () => ({
  currentComponent: 'Main'
});

const methods = {
  switchComponent(newComponent) {
    data.currentComponent = newComponent;
  }
};

const components = {
  Contact,
  Event,
  Main,
  Members,
  Offers,
  Shop
};
</script>