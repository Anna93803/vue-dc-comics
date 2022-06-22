<template>
  <div id="app">
    <TheHeader/>
    <TheJumbo/>
    <ContainerCards/>
    <TheBanner/>
    <TheFooterTop/>
    <TheFooterBottom/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheBanner from './components/TheBanner.vue';
import TheFooterTop from './components/TheFooterTop.vue';
import TheFooterBottom from './components/TheFooterBottom.vue';
import TheJumbo from './components/TheJumbo.vue';
import ContainerCards from './components/ContainerCards.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheBanner,
    TheFooterTop,
    TheFooterBottom,
    TheJumbo,
    ContainerCards
}
}
</script>

<style lang="scss">
@import './assets/css/main.scss';

</style>
