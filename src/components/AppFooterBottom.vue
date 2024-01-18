<script>
export default {
    data() {
        return {

        };
    },
    methods: {

    }
}
</script>

<template>
    <footer>
        <div class="my-container">
            <div class="footer-bottom">
                <button class="sign-button">
                    SING-UP NOW!
                </button>
                <div class="follow">
                    <span>FOLLOW US</span>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                </div>   
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer{
    background-color: rgb(48,48,48);
}
.my-container{
    padding: 20px 0;
    .footer-bottom{
        display: flex;
        justify-content: space-between;
        align-items: center;
        .sign-button{
            padding: 15px;
            font-size: 18px;
            border: 4px solid rgb(2,130,249);
            background-color: rgb(48,48,48);
            color: white;
            cursor: pointer;
        }
        .follow{
            color: rgb(2,130,249);
            font-weight: bold;
            font-size: 20px;
            display: flex;
            align-items: center;
            span{
                padding: 0 10px;
            }
            img{
                margin: 0 15px;
            }
        }
    }
}
</style>
