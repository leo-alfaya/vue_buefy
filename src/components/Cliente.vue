<template>
  <div class="columns is-multiline">
    <div class="column is-one-third" v-for="cliente in clientes" v-bind:key="cliente.id">
      <Card :cliente="cliente"></Card>
    </div>
  </div>
</template>
<script>
  import Card from './cliente/Card'

  export default {
    name: 'Cliente',
    props: ['clientes'],
    components: {
      Card
    }
  }
</script>
<style scoped lang="scss">
  
</style>
