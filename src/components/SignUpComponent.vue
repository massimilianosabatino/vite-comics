<script>
export default {}
</script>
<template>
    <button type="button">SIGN-UP NOW!</button>
</template>
<style lang="scss" scoped>
    @use "../assets/style/abstracts/variables" as *;
    @use "../assets/style/base/typo" as *;

    button {
        background-color: transparent;
        color: #fff;
        font-weight: 600;
        border: 2px solid $primary-color;
        padding: .875rem;
        @include font-family;
        cursor: pointer;
    }
</style>