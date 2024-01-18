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
    <div class="content">
        <div class="my-container">
            
                -- > Content goes here --
            
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins.scss' as *;
.my-container{
    @include container;
}

.content{
    background-color: black;
    color: white;
    >.my-container {
        padding: 60px 0;
        font-size: 30px;
    }
}
</style>
