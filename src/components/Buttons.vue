<template>
   <div class="buttons-section">
    <v-dialog
      v-model="dialog"
      width="500"
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          v-bind="attrs"
          v-on="on" class="btn-open">
         <span><img src="../assets/play.png" alt="icon play" class="img-fluid" style="vertical-align: top;"> Assistir agora </span>
        </v-btn>
      </template>

      <v-card>
       <iframe width="500" height="315" src="https://www.youtube.com/embed/ByXuk9QqQkk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </v-card>
    </v-dialog>



     <v-dialog
      v-model="dialog"
      width="500"
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          v-bind="attrs"
          v-on="on" class="btn-open btn-border">
          <span>  Assistir trailer </span>
        </v-btn>
      </template>

      <v-card>
        <iframe width="500" height="315" src="https://www.youtube.com/embed/ByXuk9QqQkk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </v-card>
    </v-dialog>
  </div>
</template>

<script>
  export default {
    name: 'Buttons',

    data: () => ({
        dialog: false,
    }),
  } 
</script>


<style scoped>

.v-btn:not(.v-btn--round).v-size--default {
    height: 50px;
    min-width: 100px;
}

.btn-open{
    width: 225px;
    background-color: #658E76 !important;
    color: #F9F9F9 !important;
    font-weight: 200;
    border-radius: unset;
      box-shadow: none;
}

.btn-open {
    transform: skew(
-25deg
);
}

.btn-open span{
    color: #f9f9f9;
    font-family: "Poppins", sans-serif;
    text-decoration: none;
    transform: skew( 
25deg
 );
}

.btn-border{
        background-color: transparent !important;
    border: 2px solid #658E76;
    box-shadow: none;
    margin-left: 1rem;
}

.buttons-section{
    margin-top:2rem;
}


@media screen and (max-width: 992px){
        .btn-border{
         display: none;
    }

.buttons-section {
    margin-bottom: 2rem;
}
     
}
</style>