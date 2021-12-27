<template>
    <div class="footer-end">
        <div class="container footer-links">
            <div class="cta">
                SIGN-UP NOW
            </div>
            <div class="links">
                <h4>FOLLOW US</h4>
                <img src="../assets/img/footer-facebook.png" alt="Facebook">
                <img src="../assets/img/footer-periscope.png" alt="Facebook">
                <img src="../assets/img/footer-pinterest.png" alt="Facebook">
                <img src="../assets/img/footer-twitter.png" alt="Facebook">
                <img src="../assets/img/footer-youtube.png" alt="Facebook">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'PostFooter'
}
</script>

<style lang="scss" scoped>
@import '../styles/variables.scss';
.footer-end {
    background-color: #303030;
    .footer-links {
        height: 80px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        .cta {
            width: 100px;
            height: 30px;
            border: 1px solid $primary_color;
            font-size: 13px;
            color: white;
            text-align: center;
            line-height: 30px;
            cursor: pointer;
        }
        .links {
            display: flex;
            align-items: center;
            h4 {
                color: $primary_color;
                padding-right: 20px;
                font-size: 13px;
            }
            img {
                width: 30px;
                cursor: pointer;
                padding-right: 10px;
            }
        }
    }
}
</style>