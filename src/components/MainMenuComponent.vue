<script>
    export default {
        data(){
            return {
                menu: [
                    {
                        name: 'characters',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'comics',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'movies',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'tv',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'games',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'collectibles',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'videos',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'fans',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'news',
                        link: '#',
                        target: '_self'
                    },
                    {
                        name: 'shop',
                        link: '#',
                        target: '_self'
                    }
                ]
            }
        }
    }
</script>
<template>
    <ul>
        <li v-for="link in menu">
            <a :href="link.link" :target="link.target">{{ link.name }}</a>
        </li>
    </ul>
</template>
<style lang="scss" scoped>
    @use "./style/variables.scss" as *;
    @use "./style/typo.scss" as *;
    ul {
        display: flex;
        list-style: none;
        font-size: 1rem;
        font-weight: 600;
        text-transform: uppercase;
        
        li {
            &:hover {
            border-bottom: 5px solid $primary-color;
            }
            a {
                color: #313131;
                text-decoration: none;
                @include font-family;
                padding-left: 2.125rem;

                &:hover {
                    color: $primary-color;
                }
            }
        }
    }
</style>