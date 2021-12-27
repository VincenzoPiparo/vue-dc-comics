<template>
    <div class="icons-contain">
        <div class="icon" v-for="icon, index in icons" :key="index">
            <img :src="require('../assets/img/' + icon.image)" :alt="icon.nameIcon">
            <h3>{{icon.nameIcon}}</h3>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PreFooter',
    data: function() {
        return {
            icons: [
                {
                    image:'buy-comics-digital-comics.png',
                    nameIcon: 'DIGITAL COMICS'
                },
                {
                    image:'buy-comics-merchandise.png',
                    nameIcon: 'DC MERCHANDISE'
                },
                {
                    image:'buy-comics-subscriptions.png',
                    nameIcon: 'SUBSCRIPTION'
                },
                {
                    image:'buy-comics-shop-locator.png',
                    nameIcon: 'COMIC SHOP LOCATOR'
                },
                {
                    image:'buy-dc-power-visa.svg',
                    nameIcon: 'DC POWER VISA'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../styles/variables.scss';
.icons-contain {
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    height: 120px;
    background-color: $primary_color;
    .icon {
        display: flex;
        align-items : center;
        h3 {
            font-size: 11px;
            font-weight: 100;
            padding-left: 10px;
            padding-right: 40px;
        }
        img {
            width: 30px;
            height: 35px;
        }
    }
}
</style>