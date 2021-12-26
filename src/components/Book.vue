<template>
    <div class="product">
        <div class="box-image">
            <img :src="bookObject.thumb" :alt="bookObject.series">
        </div>
        <h5>{{ bookObject.series }}</h5>
    </div>
</template>

<script>
export default {
    name: 'Book',
    props: ['bookObject']
}
</script>

<style lang="scss" scoped>
.product {
    width: calc( (100% / 6) - 10px );
    margin: 5px;
    padding-bottom: 20px;
    .box-image {
        display: flex;
        width: 100%;
    }
    h5 {
        color: white;
        text-transform: uppercase;
        font-size: 10px;
        padding-top: 10px;
        font-weight: 100;
    }
}
img {
    width: 100%;
}
</style>