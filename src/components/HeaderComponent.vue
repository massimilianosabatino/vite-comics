<script>
    import LogoComponent from './LogoComponent.vue';
    import MainMenuComponent from './MainMenuComponent.vue';

    export default {
        components: {
            LogoComponent,
            MainMenuComponent,
        }
    }
</script>
<template>
    <div class="container">
        <LogoComponent class="logo" />
        <MainMenuComponent class="menu"/>
    </div>
</template>
<style lang="scss" scoped>
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>