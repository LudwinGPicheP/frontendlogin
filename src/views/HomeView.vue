<template>
  <div class="home">
    <img alt="RedStone Logo" src="../assets/LogoRedStone.png">
    <HelloWorld msg="Bienvenido a RedStone"/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

export default defineComponent({
  name: 'HomeView',
  components: {
    HelloWorld,
  },
});
</script>
