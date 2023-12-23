<script>
import appHeader from './components/appHeader.vue';
import appMain from './components/appMain.vue';
import appFooter from './components/appFooter.vue';

export default{
  components: {
    appHeader,
    appMain,
    appFooter
  }
}
</script>

<template>
  <section>
    <appHeader/>
  </section>

  <section>
    <appMain/>
  </section>

  <section>
    <appFooter/>
  </section>
</template>

<style lang="scss" scoped>
 
</style>
