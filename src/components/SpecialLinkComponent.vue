<script>
    export default{
        props: {
            name: String,
            url: String,
            link: String
        }

    };
</script>
<template>
    <a :href="link">
        <div>
            <img :src="url" :alt="`Icon ${name}`">
            <div class="text">{{ name }}</div>
        </div>
    </a>
</template>
<style lang="scss" scoped>
</style>