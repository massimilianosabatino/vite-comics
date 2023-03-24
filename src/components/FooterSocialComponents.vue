<script>
    export default {}
</script>
<template>
    <div class="wrapper">
        <div class="title">FOLLOW US</div>
        <div class="icons">
            <img src="./../assets/img/footer-facebook.png" alt="Logo Facebook">
            <img src="./../assets/img/footer-twitter.png" alt="Logo Twitter">
            <img src="./../assets/img/footer-youtube.png" alt="Logo Youtube">
            <img src="./../assets/img/footer-pinterest.png" alt="Logo Pinterest">
            <img src="./../assets/img/footer-periscope.png" alt="Logo Periscope">
        </div>
    </div>
</template>
<style lang="scss" scoped>
    @use "../assets/style/abstracts/variables" as *;
    @use "../assets/style/base/typo" as *;
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