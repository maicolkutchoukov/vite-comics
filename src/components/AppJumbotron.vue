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
    <div class="jumbotron">
<!--         <img src="../assets/img/jumbotron.jpg" alt=""> -->
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins.scss' as *;
.my-container{
    @include container;
}

.jumbotron{
    background-image: url('../assets/img/jumbotron.jpg');
    background-repeat: no-repeat;
    width: 100%;
    height: 400px;
}
</style>
