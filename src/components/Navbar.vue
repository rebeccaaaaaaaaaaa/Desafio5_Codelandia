<template>
    <v-row class="align-row">
      <v-col lg="2" sm="4" md="2">
        <img src="../assets/logo.svg" alt="Logo" class="img-fluid w-70">
      </v-col>
      <v-col lg="6" sm="4" class="text-end">
          <ul class="list-nav">
            <li>
              <a href=""> <img src="../assets/facebook.png" alt="Fcebook" class="img-fluid"></a>
            </li>
             <li>
              <a href=""> <img src="../assets/instagram.png" alt="instagram" class="img-fluid"></a>
            </li>
             <li>
              <a href=""> <img src="../assets/twitter.png" alt="twitter" class="img-fluid"></a>
            </li>
             <li>
              <a href=""> <img src="../assets/youtube.png" alt="youtube" class="img-fluid"></a>
            </li>
          </ul>
      </v-col>
    </v-row>
</template>

<script>
  export default {
    name: 'Navbar',

    data: () => ({

    }),
  }
</script>

<style scoped>
.img-fluid{
  max-width: 100%;
}



.list-nav{
    text-align: end;
    list-style: none;
    padding: unset;
    margin: unset;
    display: inline-flex;
    align-items: center;
}

.list-nav li{
      margin-right: 2rem;
}

.w-70{
      width: 70%;
}

@media screen and (max-width: 992px) {
  .list-nav li {
    margin-right: 1rem;
}

.list-nav{
    margin-top: 2rem;
}

}
</style>


