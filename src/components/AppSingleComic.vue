<script>
export default {
    data() {
        return {
        };
    },
    methods:{
    },
    props: {
        singleComic : Object
    }
}
</script>

<template>
        <div class="col-lg-2 col-md-3 col-sm-4 col-6">
            <div class="my-card">
                <div class="card-image">
                <img class="img-fluid" :src="singleComic.thumb" alt="">
                </div>
                <p class="card-title">
                    {{ singleComic.series }}
                </p>
                <div class="price">
                    {{ singleComic.price }}
                </div>
            </div>
        </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins.scss' as *;
.my-card{
    height: 220px;
    margin: 0 5px;
    padding: 0 10px;
    margin-bottom: 20px;
    cursor: pointer;
    position: relative;
    &:hover .price{
            display: block;
        }
        
    .card-image{
        width: 100%;
        height: 80%;
        overflow: hidden;
    }
    .card-title{
        height: 20%;
        font-size: 11px;
        padding: 15px 0;
        text-transform: uppercase;
    }
    .price{
        position: absolute;
        top: 0px;
        padding: 40px;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.5);
        display: none;
    }
}
/* .my-card{
  width: calc((100% / 6) - 10px);
    height: 220px;
    margin: 0 5px;
    padding: 0 10px;
    margin-bottom: 20px;
    cursor: pointer;
    position: relative;
    &:hover .price{
            display: block;
        }
        
    .card-image{
        width: 100%;
        height: 80%;
        overflow: hidden;
    }
    .card-title{
        height: 20%;
        font-size: 11px;
        padding: 15px 0;
        text-transform: uppercase;
    }
    .price{
        position: absolute;
        top: 0px;
        padding: 40px;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.5);
        display: none;
    }
} */
        
</style>
