<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="container">
      <a class="navbar-item" v-for="item in items" v-bind:key="item.key">
        {{ item.text }}
      </a>
    </div>
  </nav>
</template>
<script>
export default {
  name: 'Menu',
  props: ['items']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
