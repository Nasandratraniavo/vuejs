<template>
  <div>{{ saluE }} {{ Nom }}</div>
  <div v-text="Loisir"></div>
  <div v-html="Commentaire"></div>
  <div v-html="Commentaire2"></div>
  <h2 v-bind:id="HeadingId">Mahafinaritra</h2>
  <Button v-bind:disabled="isDisabled">Press</Button>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      saluE: 'Bonjour',
      Nom: 'Nasandratra',
      Loisir: 'Batterie',
      Commentaire: '<b>Tsara ilay mitendry</b>',
      Commentaire2: `<a href="#" onclick="alert('Ho Azy irery ihany ny voninahitra')">Tsindrio ne!</a>`,
      HeadingId: 'footer',
      isDisabled: false
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
