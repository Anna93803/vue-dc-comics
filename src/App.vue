<template>
  <div id="app">
    <TheHeader/>
    <TheFooterTop/>
    <TheFooterBottom/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheFooterTop from './components/TheFooterTop.vue';
import TheFooterBottom from './components/TheFooterBottom.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooterTop,
    TheFooterBottom
}
}
</script>

<style lang="scss">
@import '@/assets/css/main.scss';

</style>
