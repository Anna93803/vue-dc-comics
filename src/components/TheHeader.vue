<template>
    <header>
        <div class="container">
            <div class="row">
                <div class="col">
                    <img src="@/assets/img/dc-logo.png" alt="logo-dc">
                </div>
                <div class="col">
                    <ul>
                        <li v-for="(link, i) in navLinks" :key="i">{{ link.name }}<a :href="link.href"></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>


<script>

export default {
    name: 'TheHeader',
    data() {
        return {
            navLinks: [
                {
                    name: 'Characters',
                    href: '#',
                },
                {
                    name: 'Comics',
                    href: '#',
                },
                {
                    name: 'Movies',
                    href: '#',
                },
                {
                    name: 'tv',
                    href: '#',
                },
                {
                    name: 'Games',
                    href: '#',
                },
                {
                    name: 'Collectibles',
                    href: '#',
                },
                {
                    name: 'Videos',
                    href: '#',
                },
                {
                    name: 'Fans',
                    href: '#',
                },
                {
                    name: 'News',
                    href: '#',
                },
                {
                    name: 'Shop',
                    href: '#',
                },
            ]
        }
    }

}
</script>


<style lang="scss" scoped>
@import '../assets/css/variables.scss';
.container {
    max-width: 1200px;
    margin: 0 auto;
    .row {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1.25rem 0;

        .col {

            ul {
                display: flex;

                li {
                    border-bottom: 2px solid transparent;
                    padding: 1.875rem 1.875rem 1.875rem 0;
                    font-weight: 500;

                    &:hover {
                        color: $ColorPrimary;
                        border-bottom: 2px solid $ColorPrimary;
                    }
                }

                li:last-child {
                    padding-right: 0;
                }
            }
        }
    }

}
</style>