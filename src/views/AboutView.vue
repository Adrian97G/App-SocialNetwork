<template>
  <div class="about container">
    <h2 class="mt-3 text-center">About Us</h2>
    <p class="text-center m-1">Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur fugit dolor distinctio dicta expedita, minus natus voluptatibus hic sapiente magnam! Voluptates libero pariatur nostrum vel porro eaque, molestiae quidem perferendis!
    </p>
    <hr />
    <div class="row">
      <img  class="col m-2 about-img" src="../assets/img/team.jpeg" alt="Imagen de equipo de trabajo">
      <img  class="col m-2 about-img" src="../assets/img/team2.jpg" alt="Imagen de equipo de trabajo">
      <img  class="col m-2 about-img" src="../assets/img/team3.jpg" alt="Imagen de equipo de trabajo">
    </div>
  </div>
</template>

<style scoped>
    .about {
      min-height: 55vh;
      max-width: 895px;
      margin: auto;
      padding: 0;
    }
    .about-img {
      display: block;
      margin-top: 2rem;
      width: 240px;
      height: auto;
      border-radius: 10%;
    }
</style>