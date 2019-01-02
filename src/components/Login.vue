<template>
  <v-container>
    <v-layout justify-center mt-5>
      <v-flex sm8 xs12>
        <v-expansion-panel>
          <v-expansion-panel-content expand-icon>
            <div slot="header" class="panel-header title">Nova Conta</div>
            <div class="panel-body">
              <v-layout align-center justify-space-around row wrap my-4>
                <h3 class="ma-2">Logar com redes sociais ou preencha o login</h3>
                <div class="ma-2">
                  <v-btn>Face</v-btn>
                  <v-btn>Insta</v-btn>
                  <v-btn>G+</v-btn>
                </div>
              </v-layout>
              <v-form>
                <v-layout row wrap>
                  <v-text-field solo class="mr-4 email-input" placeholder="Email"></v-text-field>
                  <v-text-field solo placeholder="Senha"></v-text-field>
                </v-layout>
                <v-btn block depressed class="btn-entrar">Entrar</v-btn>
                <v-btn block flat>Esqueci minha senha</v-btn>
              </v-form>
            </div>
          </v-expansion-panel-content>
          <v-expansion-panel-content expand-icon>
            <div slot="header" class="panel-header title">Registrar</div>
            <div class="panel-body">
              <v-layout align-center justify-space-around row wrap my-4>
                <h3 class="ma-2">Logar com redes sociais ou preencha o login</h3>
                <div class="ma-2">
                  <v-btn>Face</v-btn>
                  <v-btn>Insta</v-btn>
                  <v-btn>G+</v-btn>
                </div>
              </v-layout>
              <v-form>
                <v-text-field solo class='new-acc-input' placeholder="Nome"></v-text-field>
                <v-layout row wrap>
                  <v-text-field solo class='new-acc-input' placeholder="Campo teste"></v-text-field>
                  <v-text-field solo class='new-acc-input' placeholder="Campo teste"></v-text-field>
                  <v-text-field solo class='new-acc-input' placeholder="Campo teste"></v-text-field>
                  <v-text-field solo class='new-acc-input' placeholder="Campo teste"></v-text-field>
                  <v-text-field solo class='new-acc-input' placeholder="Campo teste"></v-text-field>
                  <v-text-field solo class='new-acc-input' placeholder="Campo teste"></v-text-field>
                  <v-text-field solo class='new-acc-input' placeholder="Campo teste"></v-text-field>
                </v-layout>
                <v-btn block depressed class="btn-entrar">Cadastre-se</v-btn>
              </v-form>
            </div>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({})
};
</script>

<style scoped>
.panel-header {
  margin: 1em 3em;
}
.panel-body {
  padding: 3em 6em;
  border-top: 5px solid grey;
}
.btn-entrar {
  padding: 2.5em 0;
}
.v-expansion-panel__header {
  border-bottom: 5px solid black;
}
.new-acc-input {
  margin-right: 1.5em;
}

@media (max-width: 1264px) {
  .panel-body {
    padding: 0 1em;
  }
  .email-input {
    margin-right: 0 !important;
  }
  .panel-header {
    text-align: center;
  }
}
</style>
