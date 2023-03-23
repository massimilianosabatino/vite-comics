<script>
  //Import app component
  import HeaderComponent from './components/HeaderComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import SubMenuComponet from './components/SubMenuComponet.vue';
  import FooterComponent from './components/FooterComponent.vue';
  export default {
    components: {
      HeaderComponent,
      MainComponent,
      SubMenuComponet,
      FooterComponent
    }
  }
</script>

<template>
    <HeaderComponent />
    <MainComponent />
    <SubMenuComponet />
    <FooterComponent />
</template>

<style lang="scss" scoped>

</style>
