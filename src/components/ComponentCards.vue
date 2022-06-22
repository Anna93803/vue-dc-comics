<template>
    <div class="cards">
        <img :src="imgUrl" :alt="titleImg">
        <h5>{{ titleImg }}</h5>
        <span>{{ price }}</span>
    </div>
</template>

<script>

export default {
    props: {
        imgUrl: String,
        titleImg: String,
        price:String,
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

.cards {
    position: relative;
    transition: 0.8s;

    &:hover {
            transform: scale(1.1)
    }

    img {
        width: 100%;
    }

    h5 {

        color: $ColorLight;
        font-size: .8125rem;
        text-transform: uppercase;
        font-weight: 300;
        padding-top: .9375rem;
    }

    span {
        color: $ColorLight;
        position: absolute;
        top: .3125rem;
        left: .3125rem;
        padding: .3125rem .5rem;
        background-color: $ColorPrimary;
    }
}

</style>