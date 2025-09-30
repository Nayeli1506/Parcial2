<template>
  <Formulario/>
</template>
 
<script>
import Formulario from './components/Formulario.vue';
 
export default {
  components: {
    Formulario,
  }
};
</script>
<template>
<div class="form-container">
<h2>Formulario de Registro</h2>
<form>
<div class="form-group">
<label for="nombre">Nombre:</label>
<input type="text" id="nombre" placeholder="Ingresa tu nombre" />
</div>
 
      <div class="form-group">
<label for="email">Correo electrónico:</label>
<input type="email" id="email" placeholder="ejemplo@correo.com" />
</div>
 
      <div class="form-group">
<label for="telefono">Teléfono:</label>
<input type="tel" id="telefono" placeholder="0000-0000" />
</div>
 
      <div class="form-group">
<label for="pais">País:</label>
<select id="pais">
<option>Elige una opción</option>
<option>El Salvador</option>
<option>Guatemala</option>
<option>Honduras</option>
</select>
</div>
 
      <div class="form-group">
<label>Género:</label>
<div class="radio-group">
<input type="radio" id="femenino" name="genero" />
<label for="femenino">Femenino</label>
<input type="radio" id="masculino" name="genero" />
<label for="masculino">Masculino</label>
</div>
</div>
 
      <div class="form-group">
<label for="comentarios">Comentarios:</label>
<textarea id="comentarios" rows="4" placeholder="Escribe algo..."></textarea>
</div>
 
      <button type="button">Enviar</button>
</form>
</div>
</template>
 
<style scoped>

.form-container {

  max-width: 500px;

  margin: auto;

  padding: 1rem;

  border: 1px solid #ccc;

  border-radius: 8px;

}

h2 {

  text-align: center;

}

.form-group {

  margin-bottom: 1rem;

}

label {

  display: block;

  margin-bottom: 0.3rem;

}

input,

select,

textarea {

  width: 100%;

  padding: 0.5rem;

  border-radius: 4px;

  border: 1px solid #ccc;

}

.radio-group {

  display: flex;

  gap: 1rem;

  align-items: center;

}

button {

  width: 100%;

  padding: 0.7rem;

  background-color: #007bff;

  color: white;

  border: none;

  border-radius: 4px;

}
</style>
 
<script>
export default {
  name: "Formulario"
};
</script>
 


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
