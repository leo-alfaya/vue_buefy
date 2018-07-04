<template>
  <div id="app">
    <Menu :items="items"></Menu>
  </div>
</template>

<script>
import Menu from './components/Menu'

export default {
  name: 'app',
  data: function() {
    return {
      items: [
        {id: 1, text: 'Clientes'},
        {id: 2, text: 'Projetos'},
        {id: 3, text: 'Trilhas'},
      ]
    }
  },
  components: {
    Menu
  }
}
</script>

<style lang="scss">

</style>
