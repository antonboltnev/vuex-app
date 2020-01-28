<template>
  <div class='v-main-wrapper'>
    <v-header/>
    <v-content />
  </div>
</template>

<script>
  import vContent from './page/v-content'
  import vHeader from './page/v-header'

  export default {
    name: "v-main-wrapper",
    components: {
      vContent,
      vHeader
    },
  }
</script>

<style scoped>

</style>