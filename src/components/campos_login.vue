<template>
    <div class="form-container">
        <div class="form-group">
            <label for="campoUsuario">Usuario:</label>
            <input type="text" id="campoUsuario" v-model="campoUsuario" class="form-control"
                placeholder="Ingrese su usuario" />
        </div>
        <div class="form-group">
            <label for="campoContrasena">Contraseña:</label>
            <input type="password" id="campoContrasena" v-model="campoContrasena" class="form-control"
                placeholder="Ingrese su contraseña" />
        </div>
        <div class="form-group">
            <input type="button" id="campoContrasena" v-model="botonIniciarSesion" class="form-control-button"
                value="Iniciar Sesión" />
        </div>
    </div>
</template>

<style scoped>
/* .login-form {
  display: block;
  flex-direction: column;
  max-width: 400px;
  margin: 0 auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 8px;
  background-color: #f9f9f9;
} */

.form-group {
  display: block;
  margin-bottom: 16px;
}

.form-control {
  width: 100%;
  padding: 8px;
  border: 1px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
  margin-top: 4px;
}

.form-control:focus {
  outline: none;
  border-color: #007bff;
}
</style>
