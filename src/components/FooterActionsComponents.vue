<script>
    import SignUpComponent from './SignUpComponent.vue';
    import FooterSocialComponents from './FooterSocialComponents.vue';
    
    export default {
        components: {
            SignUpComponent,
            FooterSocialComponents
        }
    }
</script>
<template>
    <div class="bg-actions">
        <div class="container">
            <SignUpComponent />
            <FooterSocialComponents />
        </div>
    </div>
</template>
<style lang="scss" scoped>
        @use "../assets/style/base/common" as *;
    .bg-actions {
        background-color: #303030;
    }
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1.875rem 0 1.1875rem 0;
        @include container;
    }
</style>