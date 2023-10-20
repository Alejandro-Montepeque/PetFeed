<template>
  <div class="container contenido-principal ">
    <div class="row">
      <!-- Columna para la imagen en pantallas medianas y grandes -->
      <div class="col-md-6 mt-2">
        <img src="https://picsum.photos/id/237/600/400" alt="" class="img-fluid mx-auto">
      </div>
      <!-- Columna para el contenido en pantallas medianas y grandes -->
      <div class="col-md-6 mt-5" id="home">
        <h1 class="texto-medio">Bienvenido a PetFeed</h1>
        <p class="textos-cortos">Bienestar en cada momento</p>
        <p class="mt-5 textos-cortos">En nuestra empresa, nos enfocamos en la automatización del cuidado de nuestros
          queridos miembros
          de la familia con el objetivo de mantener su salud y vitalidad. Porque valoramos tanto a ellos como a ti.</p>
      </div>
    </div>
    <br>
    <br>
    <br>
    <div class="pt-5" id="presentation">
      <h3 class="texto-medio">Presentación del Producto</h3>
      <p class="textos-cortos">
        Nuestro producto es un dispensador inteligente de comida el cual únicamente dispensara comida a aquellas mascotas
        que posean un collar el cual será detectado por el mismo dispensador y de esta manera surtir la comida necesaria
        también poseerá un medidor con luces led que indicara el nivel de comida del depósito del dispensador todo esto
        controlado por un Arduino Uno.
      </p>
      <div class='row'>
        <div class="col-md-6">
          <img src="@/assets/coming.png" alt="prox" width="400">
        </div>
        <div class="col-md-6">
          <img src="@/assets/coming.png" alt="prox" width="400">
        </div>
        <div class="col-md-12 mt-5">
          <div class="video-container">
            <video controls>
              <source src="@/assets/Presentacion_Petfeed.mp4" type="video/mp4">
              Tu navegador no soporta la reproducción de video.
            </video>
          </div>
        </div>
      </div>
      <P class="textos-cortos">Tu opinón nos interesa <a
          href="https://docs.google.com/forms/d/e/1FAIpQLSeT80WjueMHaVPbkcplwzMWerLEKmzPtPZB9NL2ltw-PG94xA/viewform">haz
          click aqui para participar en una encuesta sobre nuestro producto</a></P>
    </div>
    <!-- Informacion sobre nostros -->
    <div class="row pt-5" id="about_we">
      <h3 class="texto-medio">
        PetFeed
      </h3>
      <div class="col-6">
        <img src="@/assets/petfeed.png" alt="Logo" class="img-fluid mx-auto">
      </div>
      <div class="col-6">
        <img src="@/assets/pruebaf.png" alt="mascota" class="img-fluid mx-auto">
      </div>
      <p class="textos-cortos">Somos una pequeña empresa que busca proporcionar que las mascotas reciban una dieta
        equilibrada y adecuada para su salud y bienestar.</p>
      <br>
      <p class="textos-cortos text-justify">Nuestra empresa busca resolver la problemática de aquellos dueños de mascotas
        que no pueden
        estar presentes todo el tiempo para poder estar al tanto del cuidado de ellos por lo que nuestra idea de negocio
        se basa
        en un dispensador de comida automático el cual solamente funcionará si la mascota de la casa porta un collar el
        cual será detectado por el dispositivo. La idea es evitar que animales que no sean de casa por ejemplo ardillas
        ratones o mapaches roben la comida de las mascotas de la casa y de esta forma asegurarnos de que las mascotas de
        las personas no les falte comida en ningún momento mientras el dueño este ausente.
      </p>
    </div>
    <br>
    <br>
    <!-- Dropwdomn -->
    <div class="pt-5">
      <h3 class="texto-medio" id="mision_vision">Misión</h3>
      <p class="text-justify textos-cortos">Facilitar la vida de los amantes de los perros al proporcionar una solución
        innovadora y confiable para la
        alimentación automática de sus mascotas. Nuestra misión es ofrecer comodidad y tranquilidad a los dueños de
        perros, asegurando que sus compañeros peludos reciban la nutrición adecuada en los momentos justos.</p>
      <h3 class="texto-medio">Visión</h3>
      <p class="text-justify textos-cortos">
        Ser líderes en la industria de soluciones de alimentación para mascotas, creando productos tecnológicos y
        funcionales que mejoren la relación entre las personas y sus perros. Aspiramos a expandir nuestra presencia
        globalmente, contribuyendo al bienestar de las mascotas y empoderando a sus cuidadores con innovación y
        compromiso.
      </p>
      <div class="row">
        <div class="image-container">
          <img v-for="(image, index) in images" :key="index" :src="image" :class="{ active: index === currentImage }"
            alt="presentation" width="365" />
        </div>
        <div class="image-container">
          <img v-for="(image, index) in newImages" :key="index" :src="image"
            :class="{ active: index === currentNewImages }">
        </div>
      </div>
      <h3 class="texto-medio" id="values">Valores</h3>
      <ul class="text-justify textos-cortos">
        <li>
          <span class="texto-sub">Innovación:</span> Abrazamos la creatividad y buscamos constantemente formas nuevas y
          mejores de abordar las
          necesidades de las mascotas y sus dueños.
        </li>
        <li>
          <span class="texto-sub">Confianza:</span> Estamos comprometidos con la confiabilidad y la consistencia en
          nuestros productos y servicios para
          que los dueños de mascotas se sientan seguros en cada interacción con nosotros.
          Compromiso con el bienestar animal: Colocamos el bienestar y la salud de las mascotas en el centro de todo lo
          que hacemos, garantizando que nuestras soluciones contribuyan positivamente a su calidad de vida.
        </li>
        <li>
          <span class="texto-sub">Comunidad:</span> Fomentamos la creación de una comunidad en la que los amantes de los
          perros puedan conectarse,
          compartir experiencias y conocimientos relacionados con el cuidado de sus mascotas.
        </li>
      </ul>
      <h3 class="texto-medio">Revelación de nuestro producto:</h3>
      <div>
        <h1 class="texto-medio">Cuenta Regresiva</h1>
        <p class="textos-cortos">Quedan {{ days }} días, {{ hours }} horas, {{ minutes }} minutos para Nustra Gran
          Feria ANUAL y la revelación de nuestro tan esperado Producto.</p>
      </div>

      <h3 class="texto-medio" id="objective">Objetivos</h3>
      <ul class="text-justify textos-cortos">
        <li>
          Establecer alianzas con tiendas de mascotas locales o clínicas veterinarias para promocionar y demostrar el
          prototipo del dispensador de comida automático.
        </li>
        <li>
          Lanzar una versión mejorada del dispensador de comida automático con características adicionales y mejor
          funcionalidad.
        </li>
        <li>
          Establecer alianzas con tiendas de mascotas locales o clínicas veterinarias para promocionar y demostrar el
          prototipo del dispensador de comida automáticos.
        </li>
        <li>
          Expandir la presencia en el mercado y establecer alianzas estratégicas con distribuidores en otras áreas
          geográficas.
        </li>
        <li>
          Implementar una plataforma en línea para monitorear y controlar el dispensador de comida de forma remota,
          brindando a los dueños de mascotas más comodidad y tranquilidad.
        </li>
        <li>
          Convertirse en un líder reconocido en soluciones de cuidado de mascotas a nivel internacional.
        </li>
        <li>
          Desarrollar una línea de productos completa para el cuidado de mascotas, que incluya dispositivos para el
          ejercicio, monitoreo de la salud y entretenimiento.
        </li>
        <li>
          Contribuir activamente al bienestar animal a través de asociaciones con organizaciones de rescate y donaciones
          a causas relacionadas con mascotas.
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import '@/assets/CSS/Style.css'

const SECOND = 1000; // Constante para un segundo en milisegundos

export default {
  name: "bodyLanding",
  data() {
    return {
      targetDate: new Date(new Date().getFullYear(), new Date().getMonth(), 29),
      countdown: null,
      images: [
        require('@/assets/cuido.png'),
        require('@/assets/cuido2.jpg'),
        require('@/assets/cuido3.jpg'),
        require('@/assets/tecno1.jpg'),
      ],
      currentImage: 0,
      newImages: [
        require("@/assets/nuevas1.jpg"),
        require("@/assets/nuevas2.jpg"),
        require("@/assets/tecno2.jpg"),
        require("@/assets/petfeed.jpeg"),
      ],
      currentNewImages: 0,
    };
  },
  mounted() {
    this.startImageTransition();
  },
  methods: {
    startImageTransition() {
      this.rotateImages();
      this.rotateNewImages();
    },
    rotateImages() {
      this.currentImage = (this.currentImage + 1) % this.images.length;
      setTimeout(this.rotateImages, 3000);
    },
    rotateNewImages() {
      this.currentNewImages = (this.currentNewImages + 1) % this.newImages.length;
      setTimeout(this.rotateNewImages, 3500);
    },
  },
  computed: {
    days() {
      const difference = this.targetDate - new Date();
      return Math.floor(difference / (SECOND * 60 * 60 * 24));
    },
    hours() {
      const difference = this.targetDate - new Date();
      return Math.floor((difference % (SECOND * 60 * 60 * 24)) / (SECOND * 60 * 60));
    },
    minutes() {
      const difference = this.targetDate - new Date();
      return Math.floor((difference % (SECOND * 60 * 60)) / (SECOND * 60));
    },
    seconds() {
      const difference = this.targetDate - new Date();
      return Math.floor((difference % (SECOND * 60)) / SECOND);
    },
  },
  beforeUnmount() {
    clearInterval(this.countdown);
  },
};
</script>
