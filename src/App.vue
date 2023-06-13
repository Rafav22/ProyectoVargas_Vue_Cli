<template>
  <div id="app">
    <h1>Tabla de ejemplo</h1>
    <Tabla :data="datos" textColor="white" backgroundColor="blue" />
  </div>
</template>

<script>
import Tabla from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    Tabla
  },
  data() {
    return {
      datos: [
        { nombre: 'Juan', edad: 25, email: 'juan@example.com' },
        { nombre: 'María', edad: 30, email: 'maria@example.com' },
        { nombre: 'Pedro', edad: 35, email: 'pedro@example.com' }
      ]
    }
  }
}
</script>

<style>
#app {
  text-align: center;
  padding: 20px;
}
</
