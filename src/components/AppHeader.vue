<script>
export default {
    data() {
        return {
            activePage: '1',
            navbar: [
                'Characters',
                'Comics',
                'Movies',
                'Tv',
                'Games',
                'Collectibles',
                'Videos',
                'Fans',
                'News',
                'Shop'
            ],
        };
    },
    methods: {
        chageCurrentPage(i){
            this.activePage = i
        }
    }
}
</script>

<template>
    <header>
        <nav class="my-container">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
            <ul>
                <li v-for="(elem, i) in navbar" >
                    <a :class="{
                        'active' : i == activePage
                        }" href="#"
                        @click="chageCurrentPage(i)">
                            {{ elem.toLocaleUpperCase() }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
header{
    width: 100%;
}
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: white;
    img{
        padding: 20px 0;
    }
    li{
        font-size: 14px;
        display: inline-block;
        
    
        a{
            text-decoration: none;
            color: black;
            padding: 30px 10px 62px 10px;
            /* transition: all .5s ease-in-out; */

            &:hover 
            /* &.active */{
                color: blue;
            }
        }
    }            
}
.active{
    border-bottom: 8px solid blue;
}
</style>
