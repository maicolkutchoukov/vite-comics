<script>
export default {
    data() {
        return {
        };
    },
    props: {
        singleComic : Object
    }
}
</script>

<template>
    <div class="my-card">
        <div class="card-image">
        <img class="img-fluid" :src="singleComic.thumb" alt="">
        </div>
        <p class="card-title">
            {{ singleComic.series }}
        </p>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins.scss' as *;

.my-card{
  width: calc((100% / 6) - 10px);
    height: 220px;
    margin: 0 5px;
    padding: 0 10px;
    margin-bottom: 20px;
        
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
}
        
</style>
