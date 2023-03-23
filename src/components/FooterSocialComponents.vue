<script>
    export default {}
</script>
<template>
    <div class="wrapper">
        <div class="title">FOLLOW US</div>
        <div class="icons">
            <img src="./../assets/footer-facebook.png" alt="Logo Facebook">
            <img src="./../assets/footer-twitter.png" alt="Logo Twitter">
            <img src="./../assets/footer-youtube.png" alt="Logo Youtube">
            <img src="./../assets/footer-pinterest.png" alt="Logo Pinterest">
            <img src="./../assets/footer-periscope.png" alt="Logo Periscope">
        </div>
    </div>
</template>
<style lang="scss" scoped>
    @use "./style/variables.scss" as *;
    @use "./style/typo.scss" as *;
    .wrapper {
        display: flex;
        flex-wrap: nowrap;
        align-items: center;
        @include font-family;

        .title {
            color: $primary-color;
            margin-right: 1.875rem;
        }

        .icons {
            img {
                margin-left: 1.125rem;
            }
        }
    }
</style>