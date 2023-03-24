<script>
    export default{
        props: {
            name: String,
            url: String,
            taget: String
        }

    };
</script>
<template>
    <a :href="taget">
        <div>
            <img :src="url" :alt="`Icon ${name}`">
            <div class="text">{{ name }}</div>
        </div>
    </a>
</template>
<style lang="scss" scoped>
</style>