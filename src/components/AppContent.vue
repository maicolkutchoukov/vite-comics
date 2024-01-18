<script>
export default {
    data() {
        return {
            options:[
            {
                image : 'buy-comics-digital-comics.png',
                logo : 'Digital Comics'
            },
            {
                image : 'buy-comics-merchandise.png',
                logo : 'DC Merchandise'
            },
            {
                image : 'buy-comics-shop-locator.png',
                logo : 'Subscription'
            },
            {
                image : 'buy-comics-subscriptions.png',
                logo : 'Comic shop locator'
            },
            {
                image : 'buy-dc-power-visa.svg',
                logo : 'DC power visa'
            }
        ]

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
<!--                 <div v-for="(elem, i) in options" class="my-col">
                    <img :src="'../assets/img/' + elem.image" :alt="elem.logo">
                    <div>{{ elem.logo.toLocaleUpperCase() }}</div>
                </div> -->
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
    padding: 45px 0;
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
