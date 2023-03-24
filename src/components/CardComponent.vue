<script>
    export default {
        props: {
            title: String,
            url: String,
        }
    }
</script>
<template>
    <div class="single">
        <img :src="url" :alt="title">
        <h2>{{ title }}</h2>
    </div>
</template>
<script lang="scss" scoped></script>