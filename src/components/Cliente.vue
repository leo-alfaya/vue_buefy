<template>
  <div class="content">
    <section class="hero is-info">
      <div class="hero-body">
        <div class="container">
          <h1>Clientes</h1>
        </div>
      </div>
    </section>
    <div class="container">
      <div class="columns is-multiline">
        <div class="column is-one-third" v-for="cliente in clientes" v-bind:key="cliente.id">
          <Card :cliente="cliente"></Card>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  import Card from './cliente/Card'

  export default {
    name: 'Cliente',
    props: ['clientes', 'items'],
    components: {
      Card,
    }
  }
</script>
<style scoped lang="scss">
  h1 {
    color: white!important;
  }
</style>
