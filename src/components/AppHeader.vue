<script>
export default {
    data() {
        return {
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

    }
}
</script>

<template>
    <header>
        <nav class="my-container">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
            <ul>
                <!-- <li>
                    <a href="">
                        CHARACTERS
                    </a>
                </li>
                <li>
                    <a href="">
                        COMICS
                    </a>
                </li>
                <li>
                    <a href="">
                        MOVIES
                    </a>
                </li>
                <li>
                    <a href="">
                        TV
                    </a>
                </li>
                <li>
                    <a href="">
                        GAMES
                    </a>
                </li>
                <li>
                    <a href="">
                        COLLECTIBLES
                    </a>
                </li>
                <li>
                    <a href="">
                        VIDEOS
                    </a>
                </li>
                <li>
                    <a href="">
                        FANS
                    </a>
                </li>
                <li>
                    <a href="">
                        NEWS
                    </a>
                </li>
                <li>
                    <a href="">
                        SHOP
                    </a>
                </li> -->
                <li v-for="(elem, i) in navbar" >
                    <a href="#">{{ elem.toLocaleUpperCase() }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: white;
    img{
        padding: 20px 0;
    }
    ul {
        display: flex;
    }
        li{
            font-size: 14px;
        }
            a{
                text-decoration: none;
                color: black;
                padding: 30px 10px 55px 10px;

                &:hover{
                    color: blue;
                    border-bottom: 8px solid blue;
                }
            }
                
}
</style>
