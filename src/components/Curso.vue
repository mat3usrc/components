<template>
  <v-responsive class="jumbotron">
    <v-container fill-height>
      <v-layout row wrap align-center justify-space-around>
        <v-flex xs4>
          <div style='background-color: black; width: 100%  ; height: 300px;'></div>
        </v-flex>
        <v-flex xs6>
          <h1 class='mb-4'>Novo Curso</h1>
          <h3>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quia cum, labore eaque reiciendis laborum impedit vel dolorum corrupti neque iste? Quia autem ratione, laboriosam vel repellendus non eaque nemo impedit.</h3>
          <v-btn depressed right class='pa-4 mt-5'>Continuar na aula 03</v-btn>
        </v-flex>
        <v-flex xs11>
          <v-layout justify-center>
            <v-progress-linear
              background-color="blue lighten-5"
              color='blue'
              height="50"
              value="75"
            ></v-progress-linear>
          </v-layout>
        </v-flex>
      </v-layout>
    </v-container>
  </v-responsive>
</template>

<script>
export default {
  data: () => ({})
};
</script>

<style scoped>

.jumbotron {
  height: 60vh;
  background-color: lightgrey;
}

</style>