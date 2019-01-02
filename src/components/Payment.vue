<template>
  <v-container>
    <v-layout justify-center>
      <v-flex sm8 xs12>
        <v-card>
          <v-card-title class="card-title px-5">Pagamento</v-card-title>
          <v-card-text>
            <v-layout row wrap justify-space-around>
              <v-flex xs4>
                <h4 class="mb-4">Cupom de desconto</h4>
                <v-text-field solo placeholder="numero"></v-text-field>
              </v-flex>
              <v-flex xs4>
                <h4 class="mb-4">Forma de pagamento</h4>
                <v-radio-group>
                  <v-radio class='ma-2' label="teste"></v-radio>
                  <v-radio class='ma-2' label="teste"></v-radio>
                  <v-radio class='ma-2' label="teste"></v-radio>
                  <v-radio class='ma-2' label="teste"></v-radio>
                </v-radio-group>
              </v-flex>
            </v-layout>
          </v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {};
</script>

<style>
.card-title {
  border-bottom: 3px solid grey;
}
</style>
