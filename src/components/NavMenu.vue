<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-ferrari-red">
    <div class="container-fluid">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <router-link class="nav-link" to="/">Home</router-link>
        </li>
      </ul>

      <div class="navbar-brand mx-auto">
        <img src="@/assets/LogoRedStone.png" alt="Logo" class="d-inline-block align-text-top">
      </div>

      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <router-link class="nav-link" to="/landing">Landing Page</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/login">Login</router-link>
        </li>
        <!-- Agrega más rutas de interés aquí -->
      </ul>
    </div>
  </nav>
</template>

<script lang="ts" setup>

</script>

<style scoped>
.bg-ferrari-red {
  background-color: #FF2800;
  /* Rojo Ferrari */
}

.nav-link {
  color: white;
  /* Color de los enlaces */
}

.nav-link:hover {
  color: #FFD700;
  /* Color dorado al pasar el ratón por encima */
}

.navbar-brand img {
  height: 40px;
  /* Ajusta la altura del logo según sea necesario */
}
</style>
