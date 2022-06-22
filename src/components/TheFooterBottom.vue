<template>
    <div class="bg-footer-bottom">
        <div class="container">
            <div class="row">
                <div class="col">
                    <button class="btn">SING-UP NOW</button>
                </div>
                <div class="col">
                    <h4>FOLLOW US</h4>
                    <ul>
                        <li><img src="../assets/img/footer-facebook.png" alt="icons-facebook"></li>
                        <li><img src="../assets/img/footer-periscope.png" alt="icons-periscope"></li>
                        <li><img src="../assets/img/footer-pinterest.png" alt="icons-pinterest"></li>
                        <li><img src="../assets/img/footer-twitter.png" alt="icons-twitter"></li>
                        <li><img src="../assets/img/footer-youtube.png" alt="icons-youtube"></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'TheFooterBottom',
}

</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

.bg-footer-bottom {
    background-color: $ColorFooter;
    padding: 1.875rem 0;

    .row {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .col {

            .btn {
                background-color: transparent;
                color: $ColorLight;
                border: 1px solid $ColorPrimary;
                padding: .625rem;
            }

            h4 {
                font-size: 1.125rem;
                color: $ColorPrimary;
                padding-right: .9375rem;
            }
        }

        .col:last-child {
            display: flex;
            align-items: center;

            ul {
                display: flex;

                li:not(:last-child) {
                    padding-right: .9375rem;
                }
            }
        }
    }
}

</style>