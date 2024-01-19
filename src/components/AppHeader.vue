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
        <nav class="container-sm d-flex justify-content-between align-items-center">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
            <ul>
                <li v-for="(elem, i) in navbar" 
                >
                    <a href="#"
                        @click="chageCurrentPage(i)"
                        :class="{
                        'active': i == activePage
                        }">
                            {{ elem.toLocaleUpperCase() }}
                    </a>
                    <div v-if="activePage == i" class="active-page"></div>
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
    img{
        padding: 20px 0;
    }
    li{
        font-size: 14px;
        display: inline-block;
        position: relative;
        padding: 10px 0;
    
        a{
            text-decoration: none;
            color: black;
            padding: 10px 10px;
            transition: all .5s ease-in-out;
            font-weight: bold;
            
            &:hover {
                color: blue;
                background-color: lightgray;
            }
        }
    }            
}
.active-page{
    width: 100%;
    height: 7px;
    background-color: blue;
    position: absolute;
    bottom: 0;
}
.active{
    color: blue;
}
</style>
