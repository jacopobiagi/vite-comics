<script>
import appHeader from '../components/header-comp/appHeader.vue';
import appMain from '../components/main-comp/appMain.vue';
import appFooter from '../components/footer-comp/appFooter.vue';


export default{
  components: {
    appHeader,
    appMain,
    appFooter,
  }
}
</script>

<template>

  <section>
    <appHeader/>
  </section>

  <section>
    <appMain />
  </section>

  <section>
    <appFooter/>
  </section>
</template>

<style lang="scss" scoped>
 
</style>
