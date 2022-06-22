<template>
    <div class="bg-jumbo">
        <div class="container">
            <button class="btn">CURRENT SERIES</button>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

.bg-jumbo {
    background-image: url('../assets/img/jumbotron.jpg');
    position: relative;
    background-repeat: no-repeat;
    background-position: top center;
    height: 400px;

    .btn {
        background-color: $ColorPrimary;
        cursor: pointer;
        color: $ColorLight;
        position: absolute;
        bottom: -1.25rem;
        border: none;
        font-weight: 700;
        padding: .8125rem;
        transition: 0.5s;

        &:hover {
            background-color: #7da4c9;;
        }
    }
}

</style>