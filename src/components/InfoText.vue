<template>
  <article>
    <p class="creator_name">HAYAO MIYAZAKI</p>
    <h1 class="movie_name">A VIAGEM DE CHIHIRO</h1>
    <p class="description_movie">
      Chihiro chega a um mundo mágico dominado por 
      uma bruxa. Aqueles que a desobedecem são 
      transformados em animais.
    </p>
  </article>
</template>

<script>
export default {
  name: "InfoText",
  data: () => ({}),
};
</script>


<style scoped>
.creator_name {
  color: #f9f9f9;
  font-weight: bold;
  font-size: 20px;
  font-family: "Poppins", sans-serif;
}

.movie_name {
  margin: auto;
  font-size: 90px;
  font-weight: bold;
  color: #f9f9f9;
  line-height: 1;
  margin-bottom: 2rem;
  font-family: "Poppins", sans-serif;
}

.description_movie {
  color: #f9f9f9;
  font-family: "Poppins", sans-serif;
  width: 66%;
}

@media screen and (min-width: 993px) and (max-width: 1264px) {
  .movie_name {

    font-size: 60px;
 }
}

@media screen and (max-width: 992px) {
  .movie_name {
    font-size: 40px;
 }

 .description_movie[data-v-9e2d7caa] {
    width: 100%;
}
}

</style>
