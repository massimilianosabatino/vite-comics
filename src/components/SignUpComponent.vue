<script>
export default {}
</script>
<template>
    <button>SIGN-UP NOW!</button>
</template>
<style lang="scss" scoped>
    @use "./style/abstracts/variables" as *;
    @use "./style/base/typo" as *;

    button {
        background-color: transparent;
        color: #fff;
        font-weight: 600;
        border: 2px solid $primary-color;
        padding: .875rem;
        @include font-family;
    }
</style>