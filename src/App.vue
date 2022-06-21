<template>
  <div id="app">
    <TheHeader/>
    <TheFooterTop/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheFooterTop from './components/TheFooterTop.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooterTop
}
}
</script>

<style lang="scss">
@import '@/assets/css/main.scss';

</style>
