<template>
    <footer>
        <div class="bg-footer">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div>
                            <ul>
                                <li><h5>Dc Comics</h5></li>
                                <li v-for="(link, i) in linksFooter.dcComics" :key="i"><a :href="link.href">{{ link.name }} </a></li>
                                <ul>
                                    <li><h5>shop</h5></li>
                                    <li v-for="(link, i) in linksFooter.shop" :key="i"><a :href="link.href">{{ link.name }}</a></li>
                                </ul>
                            </ul>
                        </div>
                        <div>
                            <ul>
                                <li><h5>Dc</h5></li>
                                <li v-for="(link, i) in linksFooter.dc" :key="i"><a :href="link.href">{{ link.name }} </a></li>
                            </ul>
                        </div>
                        <div>
                            <ul>
                                <li><h5>Sites</h5></li>
                                <li v-for="(link, i) in linksFooter.sites" :key="i"> <a :href="link.href">{{ link.name }}</a></li>
                            </ul>
                        </div>
                    </div>
                    <div class="col">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>

export default {
    name: 'TheFooterTop',
    data() {
        return {
            linksFooter: {
                dcComics: [
                    {
                        name: 'Characters',
                        href: '#'
                    },
                    {
                        name: 'Comics',
                        href: '#'
                    },
                    {
                        name: 'Movies',
                        href: '#'
                    },
                    {
                        name: 'Tv',
                        href: '#'
                    },
                    {
                        name: 'Games',
                        href: '#'
                    },
                    {
                        name: 'Videos',
                        href: '#'
                    },
                    {
                        name: 'News',
                        href: '#'
                    },
                ],
                shop: [
                    {
                        name: 'Shop Dc',
                        href: '#'
                    },
                    {
                        name: 'Shop Dc Collectibles'
                    },
                ],
                dc: [
                    {
                        name: 'Terms of Use',
                        href : '#'
                    },
                    {
                        name: 'Ad Choices',
                        href: '#'
                    },
                    {
                        name: 'Privacy policy (New)',
                        href: '#'
                    },
                    {
                        name: 'Advertising',
                        href: '#'
                    },
                    {
                        name: 'Jobs',
                        href: '#'
                    },
                    {
                        name: 'Subscriptions',
                        href: '#'
                    },
                    {
                        name: 'Talent WorkShop',
                        href: '#'
                    },
                    {
                        name: 'CPSC Certificates',
                        href: '#'
                    },
                    {
                        name: 'Ratings',
                        href: '#'
                    },
                    {
                        name: 'Shop Help',
                        href: '#'
                    },
                    {
                        name: 'Contact Us',
                        href: '#'
                    },
                ],
                sites: [
                    {
                        name: 'DC',
                        href: '#'
                    },
                    {
                        name: 'MAD Megazine',
                        href: '#'
                    },
                    {
                        name: 'DC Kinds',
                        href: '#'
                    },
                    {
                        name: 'DC Universe',
                        href: '#'
                    },
                    {
                        name: 'DC Power Visa',
                        href: '#'
                    },
                ]
            }
        }
    }
}

</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

.bg-footer {
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: repeat;
    background-position: left center;
    .row {
        display: flex;

        .col {
            display: flex;
            gap: 3.125rem;
            padding: 3.125rem 0;

            h5 {
                padding-bottom: .625rem;
                padding-top: .375rem;
                text-transform: uppercase;
                font-size: 1rem;
                color: $ColorLight;
            }

            li {
                padding-bottom: .25rem;
                font-size: .8125rem;

                a {
                    color: $ColorGrey;
                    text-decoration: none;
                }

                &:hover {
                    text-decoration: underline;
                }
            }
        }
        .col:last-child {
            flex-grow: 1;
            background-image: url("../assets/img/dc-logo-bg.png");
            background-repeat: no-repeat;
            background-position: center right;
        }
    }
}

</style>