<template>
  <header style="height: 50px; border-bottom: 1px solid black;">
    <div style="display: flex; justify-content: space-around; align-items: center; height: 100%;">
      <button @click="abrirPestañaEducador()">Educador</button>
      <button @click="abrirNuevaPestana()">Grupo</button>
      <button @click="abrirNuevaPestana()">Cliente</button>
      <button @click="abrirNuevaPestana()">Proveedor</button>
      <button @click="abrirNuevaPestana()">Contrato</button>
    </div>
  </header>
   
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

<script lang="ts">
export default {
  methods: {
    abrirNuevaPestana() {
      window.open('https://www.google.com', '_blank');
    },
    abrirPestañaEducador() {
      window.open('@/src/ventanas/Educador.html', '_blank');
    }
  }
}

</script>