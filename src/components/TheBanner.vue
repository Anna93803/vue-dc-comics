<template>
    <div class="bg-banner">
        <div class="container">
            <div class="banner-cards">
                <ul>
                    <li v-for="(link, i) in linkBanner" :key="i">
                        <a :href="link.href">
                            <img :src="'@/assets/img/' + link.src" alt="">
                            <!-- <img src="@/assets/img/buy-comics-digital-comics.png" alt=""> -->
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
                    alt: 'Digital Comics',
                    href: '#'
                },
                {
                    name: 'DC Merchandise',
                    src: 'buy-comics-merchandise.png',
                    alt: 'DC Merchandise',
                    href: '#'
                },
                {
                    name: 'Subscription',
                    src: 'buy-comics-subscriptiona.png',
                    alt: 'Subscription',
                    href: '#'
                },
                {
                    name: 'Comics Shop locator',
                    src: 'buy-comics-shop-locator.png',
                    alt: 'Shop Locator',
                    href: '#'
                },
                {
                    name: 'Dc Power Visa',
                    src: 'buy-dc-power-visa',
                    alt: 'DC Merchandise',
                    href: '#'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/assets/css/variables.scss';

.bg-banner {
    background-color: $ColorPrimary;
    padding: 1.875rem 0;

    .banner-cards {
        
        ul {
            display: flex;
            justify-content: space-between;

            li {
                max-width: 45px;
            }

            li a {
                display: flex;
                align-items: center;
                text-decoration: none;
                color: $ColorLight;
                font-size: .75rem;
                font-weight: 300;
                text-transform: uppercase;

                img {
                    width: 100%;
                    margin-right: .9375rem;
                }
            }
        }
    }
}

</style>