<template>
  <div class="container">
    <div class="row">
      <!-- Columna para la imagen en pantallas medianas y grandes -->
      <div class="col-md-6 mt-2">
        <input type="image" src="https://picsum.photos/id/237/600/400" alt="" width="550" height="400">
      </div>
      <!-- Columna para el contenido en pantallas medianas y grandes -->
      <div class="col-md-6 mt-5">
        <h1 class="texto-medio">Bienvenido a PetFeed</h1>
        <p class="textos-cortos">Bienestar en cada momento</p>
        <p class="mt-5">En nuestra empresa, nos enfocamos en la automatización del cuidado de nuestros queridos miembros de la familia con el objetivo de mantener su salud y vitalidad. Porque valoramos tanto a ellos como a ti, hemos creado este dispositivo inteligente especialmente para ti</p>
      </div>
    </div>
  </div>
</template>

<script>
import '@/assets/CSS/Style.css'
export default {
  name: "BodyJumbotron",
};
</script>
