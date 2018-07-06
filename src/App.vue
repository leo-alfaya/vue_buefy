<template>
  <div id="app">
    <section class="content">
      <Menu :items="items"></Menu>
      <Cliente :clientes="clientes"></Cliente>
    </section>
  </div>
</template>

<script>
import Menu from './components/Menu'
import Cliente from './components/Cliente'

export default {
  name: 'app',
  data: function() {
    return {
      items: [
        {id: 1, text: 'Home'},
      ],
      clientes: [
        {id: 1, nome: 'Cliente_1'},
        {id: 2, nome: 'Cliente_2'},
        {id: 3, nome: 'Cliente_3'},
        {id: 4, nome: 'Cliente_4'},
        {id: 5, nome: 'Cliente_5'},
        {id: 6, nome: 'Cliente_6'},
        {id: 7, nome: 'Cliente_7'},
        {id: 8, nome: 'Cliente_8'},
        {id: 9, nome: 'Cliente_9'},
      ]
    }
  },
  components: {
    Menu,
    Cliente
  }
}
</script>

<style lang="scss">
  body {
    width: 100%;
    height: 100%;
  }

  .content {
    width: 100%;
    height: 100%;
  }
</style>
