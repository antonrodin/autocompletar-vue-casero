<template>
  <div id="app">
    <autocomplete :items="nombres" @selecionado="mostrarSeleccionado"></autocomplete>
  </div>
</template>

<script>
import Autocomplete from './components/Autocomplete.vue'

export default {
  name: 'App',
  
  components: {
    Autocomplete
  },

  data() {

    return {

      nombres: [
        'Anton',
        'Alberto',
        'Lucia',
        'Tatnia',
        'Sergio',
        'Pedro'
      ]

    }

  },

  methods: {
    mostrarSeleccionado(nombre) {
      console.log(nombre);
    }
  }

}
</script>