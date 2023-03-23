<script>
import SecondaryMenuComponent from './SecondaryMenuComponent.vue';
    export default {
        components: {
            SecondaryMenuComponent
        }
    }
</script>
<template>
    <div class="bg">
        <div class="secondary-menu">
            <div class="menu">
                <SecondaryMenuComponent/>
            </div>
            <div class="logo-img">
                <img src="./../assets/dc-logo-bg.png" alt="Logo DC">
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    @use "./style/variables.scss" as *;
    @use "./style/common.scss" as *;

    .bg {
        background-image: url(./../assets/footer-bg.jpg);
        .secondary-menu {
            display: flex;
            justify-content: space-between;
            overflow: hidden;
            max-height: 23.125rem;
            @include container;
            .menu {
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
                padding-top: 2.5rem;
                padding-bottom: 2.5rem;
            }
            .logo-img {
                align-self: center;
                img {
                    display: block;
                }
            }
        }
    }
</style>