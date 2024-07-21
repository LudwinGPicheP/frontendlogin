<template>
  <div class="home">
    <img id="logo" alt="RedStone Logo" src="../assets/LogoRedStone.png">
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

<style scoped>
.home {
    background-color: black;
    height: 100vh; /* Para asegurar que cubra toda la vista */
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
#logo {
    display: block;
    width: 100px;
    height: 100px;
}

</style>
