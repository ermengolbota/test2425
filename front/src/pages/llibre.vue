<template>
  <div>
    <h1>URL del back que canvia en funció del mode: {{ URL_BACK }}</h1>
    <p>El valor de la variable s'agafa d'un fitxer o un altre en funció del mode (dev, build...)

    </p>
    <h2>Fitxers possible</h2>
    <p>El normal és tenir els tres fitxers</p>
    <ul>
      <li><code>.env:</code>Hauria de contenir les claus, sense valor. Aquest fitxer SÍ que puja al github</li>
      <li><code>.env.locat: </code>Serveix per definir l'entorn de desenvolupament. Cada desenvolupador hi posa els seus
        valors. NO puja al gthub</li>
      <li><code>.env.production: </code>Es llegeix quan es fa <code>npm run build</code> i per tant, l'aplicació
        resultant que està a la carpeta dist utilitza aquests valors</li>
    </ul>

  </div>
</template>

<script>
export default {
  data() {
    return {
      URL_BACK: import.meta.env.VITE_URL_BACK // Definida En el fitxer .env i/o .env.local, a l'arrel del vue
    };
  },
}
</script>

<style scoped>
/* Afegir estils si és necessari */
</style>
