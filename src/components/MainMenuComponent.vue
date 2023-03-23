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
        align-items: center;
        list-style: none;
        font-size: 1rem;
        font-weight: 600;
        text-transform: uppercase;
        height: 100%;
        
        li {
            display: flex;
            align-items: center;
            height: 100%;
            position: relative;
            &:hover::before {
                content: '';
                position: absolute;
                left: 0;
                bottom: 0;
                height: 5px;
                width: 100%;
                background-color: $primary-color;
            }

            a {
                color: #313131;
                text-decoration: none;
                @include font-family;
                margin: 0 .9375rem;
            }
        }
    }
</style>