<template>
  <header>
    <h1>{{ saluE }} {{ Nom }}</h1>
    <p v-text="Loisir"></p>
  </header>

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      saluE: 'Bienvenue',
      Nom: 'Mr Gaetan',
      Loisir: 'Exercice d\'application Docker, creation container et image',
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');
*{
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
body{
  font-family: 'Open sans', sans-serif;
  background: #fff;
}
header{
  display: flex;
  height: 100vh;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #fff;
}
header::before{
  content: '';
  background: url('./assets/trano.jpg') no-repeat center center/cover;
  top: 0;
  left: 0;
  position: absolute;
  opacity: 0.9;
  width: 100%;
  height: 100%;
  z-index: -1;
}
header > h1{
  font-size: 4rem;
  color: rgb(4, 135, 187);
  padding: 1rem 0;
  text-shadow: 1px 1px #fff;
}
header > p{
  font-weight: 600;
  font-size: 1.8rem;
}
</style>
