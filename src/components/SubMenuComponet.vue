<script>
import SpecialLinkComponent from './SpecialLinkComponent.vue';
export default {
    components: {
        SpecialLinkComponent
    },
    data() {
        return {
            cards: [
                {
                    name: 'digital comics',
                    url: './src/assets/img/buy-comics-digital-comics.png',
                    link: '#'
                },
                {
                    name: 'dc merchandise',
                    url: './src/assets/img/buy-comics-merchandise.png',
                    link: '#'
                },
                {
                    name: 'subscription',
                    url: './src/assets/img/buy-comics-subscriptions.png',
                    link: '#'
                },
                {
                    name: 'comic shop locator',
                    url: './src/assets/img/buy-comics-shop-locator.png',
                    link: '#'
                },
                {
                    name: 'dc power visa',
                    url: './src/assets/img/buy-dc-power-visa.svg',
                    link: '#'
                },
            ]
        }
    }
}
</script>
<template>
    <div class="sub-menu">
        <div v-for="element in cards">
            <a :href="element.link">
                <div>
                    <img :src="element.url" :alt="`Icon ${element.name}`">
                    <div class="text">{{ element.name }}</div>
                </div>
            </a>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    @use "../assets/style/abstracts/variables" as *;
    .sub-menu {
        height: 155px;
        background-color: $primary-color;
        display: flex;
        justify-content: space-between;

        div {
            display: flex;
            flex-wrap: nowrap;
            align-items: center;
        }
    }

</style>