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
                    target: '#'
                },
                {
                    name: 'dc merchandise',
                    url: './src/assets/img/buy-comics-merchandise.png',
                    target: '#'
                },
                {
                    name: 'subscription',
                    url: './src/assets/img/buy-comics-subscriptions.png',
                    target: '#'
                },
                {
                    name: 'comic shop locator',
                    url: './src/assets/img/buy-comics-shop-locator.png',
                    target: '#'
                },
                {
                    name: 'dc power visa',
                    url: './src/assets/img/buy-dc-power-visa.svg',
                    target: '#'
                },
            ]
        }
    }
}
</script>
<template>
    <div class="sub-menu">
        <!-- <div v-for="element in cards"> -->
            <!-- <a :href="element.target">
                <div>
                    <img :src="element.url" :alt="`Icon ${element.name}`">
                    <div class="text">{{ element.name }}</div>
                </div>
            </a> -->
        <div class="wrapper">
            <SpecialLinkComponent v-for="element in cards"
                :name="element.name"
                :url="element.url"
                :link="element.target"
                />
        </div>
        <!-- </div> -->
    </div>
</template>
<style lang="scss" scoped>
    @use "../assets/style/abstracts/variables" as *;
    @use "../assets/style/base/common.scss" as *;

    .sub-menu {
        height: 155px;
        background-color: $primary-color;

        .wrapper {
            @include container;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        
        :deep(div) {
            display: flex;
            flex-wrap: nowrap;
            align-items: center;
            a {
                flex-basis: calc(100% / 5);
                &:hover{
                    animation: 0.5s infinite alternate bounce;
                }
                
                
                div {
                    justify-content: center;
                    color: #fff;
                    text-transform: uppercase;
                    font-weight: 600;
                }
            }
            img {
                max-width: 3.4375rem;
                max-height: 3.4375rem;
                margin-right: .75rem;
            }
        }
    }



</style>