<template>
    <div class="main-cont">
        <div class="container">
            <span>
                CURRENT SERIES
            </span>
        </div>
        <ComicsBookList/>
    </div>
</template>

<script>
import ComicsBookList from "./ComicsBookList.vue";
export default {
    name: "Main",
    components: {
        ComicsBookList
    },
}
</script>

<style scoped lang="scss">
@import '../styles/variables.scss';
.container {
    position: relative;
    span {
    padding: 10px 20px;
    color: white;
    cursor: pointer;
    font-size: 18px;
    background-color: $primary_color;
    position: absolute;
    top: -20px;
    left: 0;
    }
}
</style>