<template>
  <div class="container">
    <div class="row">
      <div
        id="carouselExampleCaptions"
        class="carousel slide col-12" 
        data-ride="carousel"
      >
        <ol class="carousel-indicators">
          <li
            data-target="#carouselExampleCaptions"
            data-slide-to="0"
            class="active"
          ></li>
          <li data-target="#carouselExampleCaptions" data-slide-to="1"></li>
          <li data-target="#carouselExampleCaptions" data-slide-to="2"></li>
        </ol>

        <div class="carousel-inner">
          <div class="carousel-item active bg-light">
            <img
              class="rounded mx-auto d-block"
              src="https://placeimg.com/1000/480/animal"
              alt="Responsive image"
            />
            <div class="carousel-caption d-none d-md-block">
              <h5 class="text-white">Animales sorprendentes</h5>
              <p class="text-white">Descubre sitios únicos y maravillosos</p>
            </div>
          </div>

          <div class="carousel-item bg-light">
            <img
              class="rounded mx-auto d-block"
              src="https://placeimg.com/1000/480/nature"
              alt="Responsive image"
            />
            <div class="carousel-caption d-none d-md-block">
              <h5 class="text-white">Naturaleza por explorar</h5>
              <p class="text-white">Descubre sitios únicos y maravillosos</p>
            </div>
          </div>

          <div class="carousel-item bg-light">
            <img
              class="rounded mx-auto d-block"
              src="https://placeimg.com/1000/480/arch"
              alt="Responsive image"
            />
            <div class="carousel-caption d-none d-md-block">
              <h5 class="text-white">Arquitectura fascinante</h5>
              <p class="text-white">Descubre sitios únicos y maravillosos</p>
            </div>
          </div>

          <a
            class="carousel-control-prev bg-light"
            href="#carouselExampleCaptions"
            role="button"
            data-slide="prev"
          >
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
          </a>
          <a
            class="carousel-control-next bg-light"
            href=" #carouselExampleCaptions"
            role="button"
            data-slide="next"
          >
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Carrusel",
  props: ["Carrusel"],
  data() {
    return {};
  },
};
</script>

<style scoped>
</style>
