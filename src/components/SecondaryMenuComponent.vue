<script>
export default {
    data() {
        return {
            menu: [
                {
                    section: 'DC COMICS',
                    link: '#',
                    target: '_self',
                    linkList: [
                        {
                            name: 'Characters',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Comics',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Movies',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'TV',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Games',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Videos',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'News',
                            link: '#',
                            target: '_self'
                        },
                    ]
                },
                {
                    section: 'SHOP',
                    link: '#',
                    target: '_self',
                    linkList: [
                        {
                            name: 'Shop DC',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Shop DC Collectibles',
                            link: '#',
                            target: '_self'
                        },
                    ]
                },
                {
                    section: 'DC',
                    link: '#',
                    target: '_self',
                    linkList: [
                        {
                            name: 'Terms Of Use',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Privacy policy (New)',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Ad Choices',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Advertising',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Jobs',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Subscriptions',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Talent Workshops',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'CPSC Certificates',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Ratings',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Shop Help',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'Contact Us',
                            link: '#',
                            target: '_self'
                        },
                    ]
                },
                {
                    section: 'SITES',
                    link: '#',
                    target: '_self',
                    linkList: [
                        {
                            name: 'DC',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'MAD Magazine',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'DC Kids',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'DC Universe',
                            link: '#',
                            target: '_self'
                        },
                        {
                            name: 'DC Power Visa',
                            link: '#',
                            target: '_self'
                        },
                    ]
                },
            ]
        }
    }
}
</script>
<template>
    <ul v-for="section in menu" class="category">
        <li>
            <a :href="section.link" :target="section.target">
                {{ section.section }}
            </a>
            <ul class="link">
                <li v-for="link in section.linkList">
                    <a :href="link.link" :target="link.target">
                        {{ link.name }}
                    </a>
                </li>
            </ul>
        </li>
    </ul>
</template>
<style lang="scss" scoped>
    @use "./style/variables.scss" as *;
    @use "./style/typo.scss" as *;

    ul {
        display: flex;
        flex-direction: column;
        list-style: none;
        font-size: 1rem;
        font-weight: 600;
        text-transform: uppercase;
        margin-right: 1.25rem;
        
        li {

            a {
                color: #FFF;
                text-decoration: none;
                @include font-family;

            }
        }

        ul {
            list-style: none;
            font-size: .75rem;
            font-weight: 400;
            text-transform: none;
            margin-top: 1.25rem;
            margin-bottom: 1.25rem;
            
            li {
                margin-bottom: .0625rem;
                a {
                    color: #797979;
                }
            }
        }        
    }
</style>