<template>
  <div class='v-content'>
    <v-catalog/>
  </div>
</template>

<script>
  import vCatalog from '../catalog/v-catalog'

  export default {
    name: "v-content",
    components: {
      vCatalog
    },
    data() {
      return {}
    },
  }
</script>

<style scoped>

</style>