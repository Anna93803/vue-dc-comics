<template>
    <header>
        <div class="container">
            <div class="row">
                <div class="col">
                    <img src="../assets/img/dc-logo.png" alt="logo-dc">
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
.row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    // padding: 1.25rem 0;
    height: 140px;

    .col {

        ul {
            display: flex;
            height: 140px;

            li {
                border-bottom: 2px solid transparent;
                text-transform: uppercase;
                font-weight: 500;
                line-height: 8.75rem;
                padding-right: 1.875rem;

                &:hover {
                    color: $ColorPrimary;
                    border-bottom: 4px solid $ColorPrimary;
                }
            }

            li:last-child {
                padding-right: 0;
            }
        }
    }
}

</style>