<template>
  <div class='v-catalog'>
    <v-catalog-item />
  </div>
</template>

<script>
  import vCatalogItem from './v-catalog-item'

  export default {
    name: "v-catalog",
    components: {
      vCatalogItem
    },
    data() {
      return {}
    },
  }
</script>

<style>
  .v-catalog {
    margin-top: 50px;
    padding: 16px;
    display: flex;
    justify-content: center;
  }
</style>