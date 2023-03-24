<script>
    export default {}
</script>
<template>
    <div class="wrapper">
        <div class="title">FOLLOW US</div>
        <div class="icons">
            <a href="#" target="_blank"><img src="./../assets/img/footer-facebook.png" alt="Logo Facebook"></a>
            <a href="#" target="_blank"><img src="./../assets/img/footer-twitter.png" alt="Logo Twitter"></a>
            <a href="#" target="_blank"><img src="./../assets/img/footer-youtube.png" alt="Logo Youtube"></a>
            <a href="#" target="_blank"><img src="./../assets/img/footer-pinterest.png" alt="Logo Pinterest"></a>
            <a href="#" target="_blank"><img src="./../assets/img/footer-periscope.png" alt="Logo Periscope"></a>
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
            font-weight: 600;
            margin-right: 1.875rem;
        }

        .icons {
            img {
                margin-left: 1.125rem;
            }
        }
    }
</style>