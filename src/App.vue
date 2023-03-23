<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  export default {
    components: {
      HeaderComponent,
      MainComponent
    }
  }
</script>

<template>
  <div class="container">
    <HeaderComponent />
    <MainComponent />
  </div>
</template>

<style lang="scss" scoped>
  .container {
    max-width: 80rem;
    margin: auto;
  }
</style>
