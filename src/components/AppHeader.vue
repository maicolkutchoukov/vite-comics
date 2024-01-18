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
    <header>
        <nav class="my-container">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
            <ul>
                <li>
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
    padding: 20px 0;
    background-color: white;

    ul {
        display: flex;
    }
        li{
            padding: 10px;
        }
            a{
                text-decoration: none;
                color: black;
                padding: 50px 10px;

                &:hover{
                    color: blue;
                    border-bottom: 8px solid blue;
                }
            }
                
}
</style>
