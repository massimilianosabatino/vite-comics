<script>
import SecondaryMenuComponent from './SecondaryMenuComponent.vue';
import FooterActionsComponents from './FooterActionsComponents.vue';

    export default {
        components: {
            SecondaryMenuComponent,
            FooterActionsComponents
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
                <img src="./../assets/img/dc-logo-bg.png" alt="Logo DC">
            </div>
        </div>
    </div>
    <FooterActionsComponents />
</template>
<style lang="scss" scoped>
    @use "../assets/style/abstracts/variables" as *;
    @use "../assets/style/base/common" as *;

    .bg {
        background-image: url(./../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
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