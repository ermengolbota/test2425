<template>
  <v-layout class="rounded rounded-md">
    <v-app-bar title="Application bar"></v-app-bar>

    <v-navigation-drawer>
      <v-list>
        <v-list-item title="Navigation drawer"></v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-main class="align-center justify-center" style="min-height: 300px;">

      <h1>Exemple d'aplicació que mostra l'ús de rutes, i també de les variables d'entorn</h1>

      <p> Per veure un <router-link to="/llibre">llibre</router-link> utilitzem una ruta cap a la pàgina que hem creat a
        pages. Ho fem amb el component <code> &lt;router-link to="page"&gt; </code></p>
      <p>Per accedir al back fem servir una variable d'entorn que canvia de valor en funció del mode</p>
      
    </v-main>
  </v-layout>

</template>

<script setup>

</script>
