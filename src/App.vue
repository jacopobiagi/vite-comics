<script>
import appHeader from './components/appHeader.vue'

export default{
  components: {
    appHeader
  }
}
</script>

<template>
  <section>

    <appHeader msg="vite + vue"/>
  </section>
</template>

<style lang="scss" scoped>
  *{
    padding: 0;
    margin: 0!important;
    box-sizing: border-box;
  }

  body{
    margin: 0!important;
  }
</style>
