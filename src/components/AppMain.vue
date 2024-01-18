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
    <main>
        <div class="my-container">
            <div class="my-row">
                <div class="my-col">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <div>DIGITAL COMICS</div>
                </div>
                <div class="my-col">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <div>DC MERCHANDISE</div>
                </div>
                <div class="my-col">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <div>SUBSCRIPTION</div>
                </div>
                <div class="my-col">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <div>COMIC SHOP LOCATOR</div>
                </div>
                <div class="my-col">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <div>DC POWER VISA</div>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins.scss' as *;
main{
    background-color: #0282F9;
}
.my-row {
    display: flex;
    justify-content: center;
    padding: 30px 0;
        .my-col{
            width: calc(100% / 5);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            img{
                width: 20%;
            }
            div{
                display: inline-block;
                padding: 20px;
            }
}
}


</style>
