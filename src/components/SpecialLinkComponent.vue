<script>
    export default{};
</script>
<template>
    <a :href="element.link">
        <div>
            <img :src="element.url" :alt="`Icon ${element.name}`">
            <div class="text">{{ element.name }}</div>
        </div>
    </a>
</template>
<style lang="scss" scoped>
</style>