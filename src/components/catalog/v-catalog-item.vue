<template>
  <div class='v-catalog-item'>
    <img src="../../assets/logo.png" alt="">
    <p>Курс по Vue.js</p>
    <br>
    <p>10 000 ₽</p>
    <button @click="btnClick" class="to_cart">Add to cart</button>
  </div>
</template>

<script>
  import {mapGetters, mapActions} from 'vuex'

  export default {
    name: "v-catalog-item",
    props: {},
    data() {
      return {}
    },
    computed: {
      ...mapGetters([
        'DROPDOWN_STATE'
      ])
    },
    methods: {
      ...mapActions([
        'TOGGLE_DROPDOWN'
      ]),
      btnClick() {
        this.TOGGLE_DROPDOWN()
      }
    }
  }
</script>

<style lang="scss">
  .v-catalog-item {
    flex-basis: 25%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 16px;
    box-shadow: 0px 5px 12px 0px #9c9c9c;
    color: #2d2d2d;
  }
</style>