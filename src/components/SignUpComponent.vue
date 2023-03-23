<script>
export default {}
</script>
<template>
    <button>SIGN-UP NOW!</button>
</template>
<style lang="scss" scoped>
    @use "./style/variables.scss" as *;
    @use "./style/typo.scss" as *;

    button {
        background-color: transparent;
        color: #fff;
        font-weight: 600;
        border: 2px solid $primary-color;
        padding: .875rem;
        @include font-family;
    }
</style>