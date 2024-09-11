<script>

export default {
    data() {
        return {

        }
    },

    props: {
        products: Object
    }
}
</script>

<template>
    <div class="card-film">
        <div>
            <img :src="products.thumb" :alt="products.series">
        </div>
        <h3>
            {{products.series}}
        </h3>
    </div>
</template>

<style lang="scss" scoped>
.card-film{
    width: calc(100% / 6 );
    padding: 10px;

    img {
        width: 100%;
        height: 190px;
    }


    h3 {
        color: white;
        padding: 10px;
        font-size: 15px;
        
    }
}
</style>
