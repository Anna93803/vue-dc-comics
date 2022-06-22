<template>
    <div class="bg-banner">
        <div class="container">
            <div class="banner-cards">
                <ul>
                    <li v-for="(link, i) in linkBanner" :key="i">
                        <a :href="link.href">
                            <img :src="require('../assets/img/' + link.src)" :alt="link.name">
                            <h4>{{ link.name }}</h4>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TheBanner',
    data () {
        return {
            linkBanner: [
                {
                    name: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png',
                    href: '#'
                },
                {
                    name: 'DC Merchandise',
                    src: 'buy-comics-merchandise.png',
                    href: '#'
                },
                {
                    name: 'Subscription',
                    src: 'buy-comics-subscriptions.png',
                    href: '#'
                },
                {
                    name: 'Comics Shop locator',
                    src: 'buy-comics-shop-locator.png',
                    href: '#'
                },
                {
                    name: 'Dc Power Visa',
                    src: 'buy-dc-power-visa.svg',
                    href: '#'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

.bg-banner {
    background-color: $ColorPrimary;
    padding: 1.875rem 0;

    .banner-cards {
        
        ul {
            display: flex;
            justify-content: space-around;
            align-items: center;

            li a {
                display: flex;
                align-items: center;
                text-decoration: none;
                color: $ColorLight;
                font-size: .75rem;
                font-weight: 300;
                text-transform: uppercase;

                img {
                    max-width: 50px;
                    margin-right: .9375rem;
                }

                &:hover {
                    transform: scale(1.1);
                }

            }
        }
    }
}

</style>