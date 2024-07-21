<template>
  <div class="d-flex justify-content-center align-items-center vh-100">
    <div class="card p-4 shadow-lg" style="max-width: 400px; width: 100%;">
      <h3 class="text-center mb-4">Iniciar Sesión</h3>
      <form @submit.prevent="onSubmit">
        <div class="mb-3">
          <label for="email" class="form-label">Correo Electrónico</label>
          <input
            type="email"
            class="form-control"
            id="email"
            v-model="email"
            required
          />
        </div>
        <div class="mb-3">
          <label for="password" class="form-label">Contraseña</label>
          <input
            type="password"
            class="form-control"
            id="password"
            v-model="password"
            required
          />
        </div>
        <button type="submit" class="btn btn-primary w-100">Iniciar Sesión</button>
      </form>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue';

const email = ref<string>('');
const password = ref<string>('');

const onSubmit = () => {
  // Aquí puedes manejar el inicio de sesión
  console.log('Correo Electrónico:', email.value);
  console.log('Contraseña:', password.value);
};
</script>

<style scoped>
.vh-100 {
  min-height: 100vh;
}
</style>
