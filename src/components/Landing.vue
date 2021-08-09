<template>
  <v-container>
    <Navbar />
    <v-row class="align-row mobile-reverse mt">
      <v-col lg="6">
          <InfoText />
          <Buttons />
      </v-col>
      <v-col lg="6">
         <Ilustration />
      </v-col>
    </v-row>
  </v-container>
</template>


<script>

  import Navbar from './Navbar.vue';
  import Ilustration from './Ilustration.vue'
  import InfoText from './InfoText.vue'
  import Buttons from './Buttons.vue'

  export default {
    name: 'Landing',
    components:{
      Navbar,
      Ilustration,
      InfoText,
      Buttons
    },
    data: () => ({

    }),
  }
</script>

<style scoped>

body{
 font-family: 'Poppins', sans-serif;
}

.w-70{
      width: 70%;
}

.w-100{
      width: 100%;
}

.align-row{
    justify-content: space-between;
    align-items: center;
}

.mt{
      margin-top: 2.5rem !important;
}

@media (max-width: 992px){
  .mobile-reverse {
    flex-direction: column-reverse;
  }
}
</style>