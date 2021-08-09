<template>
  <v-app>
    <v-main>
      <Landing/>
    </v-main>
  </v-app>
</template>

<script>
import Landing from './components/Landing';

export default {
  name: 'App',
  components: {
    Landing
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="css">
.v-main{
    background: linear-gradient(130.02deg, #628E75 0.66%, #1A4855 83.32%);
  }

  @media screen  and (max-width: 992px){
    .v-main{
         padding: 0 1rem !important;
    }
  }
</style>
