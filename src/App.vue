<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <!--  -->
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>SI Festi'neuch</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <v-container>
         <p class="text-h4 text--primary text-center">Gestion de flux de la porte d'entrée</p>
       <v-card
          class="mx-auto"
          max-width="500"
        >
          <v-card-text>
            <p class="text-h5 text--primary">
              Prédiction du flux
            </p>            
            <div>Jeudi, 26.06</div>
            <div>19:32</div>
            <p class="text-h5 text--primary">
              Demande de bénévoles à l'entrée
            </p>
            <v-alert type="error">
              Besoin de mobilisation : 2 bénévoles
            </v-alert>
            <div class="text--primary font-weight-medium">
              arrivée en provenance de : Fribourg<br>
              estimation de : 500 personnes
            </div>
          </v-card-text>
        </v-card>
         <v-card
          class="mx-auto"
          max-width="500"
        >

          <v-card-text class="mt-12">
            <p class="text-h5 text--primary">
              Prédiction du flux
            </p>            
            <div>Jeudi, 26.06</div>
            <div>21:10</div>
            <p class="text-h5 text--primary">
              Demande de bénévoles à l'entrée
            </p>
            <v-alert type="info">
              Flux contrôlé
            </v-alert>
            <div class="text--primary font-weight-medium">
              arrivée en provenance de : Lausanne<br>
              estimation de : 10 personnes
            </div>
          </v-card-text>
        </v-card>
      
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    data: () => ({ drawer: null }),
  }
</script>