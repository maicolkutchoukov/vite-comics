<script>
export default {
    data() {
        return {
            comics:[
                'Characters',
                'Comics',
                'Movies',
                'Tv',
                'Games',
                'Videos',
                'News'
            ],
            dc:[
                'Term Of Use',
                'Privacy policy (New)',
                'Ad Choise',
                'Advertising',
                'Jobs',
                'Subscription',
                'Talent Workshops',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ],
            shop:[
                'Shop DC',
                'Shop DC Collectibles'
            ],
            sites:[
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa',
            ]
        };
    },
    methods: {

    }
}
</script>

<template>
    <footer>
        <div class="my-container">
            <div class="my-row">
                <div class="my-col-5">
                    <div class="my-row">
                        <div class="my-col">
                            <div>
                                <span>
                                    DC COMICS
                                </span>
                                <ul>
                                    <li v-for="(elem, i) in comics">
                                        <a href="">{{ elem }}</a>
                                    </li>
                                </ul>
                            </div>
                            <div>
                                <span>
                                    SHOP
                                </span>
                                <ul>
                                    <li v-for="elem in shop">
                                        <a href="">
                                            {{ elem }}
                                        </a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                        <div class="my-col">
                            <div>
                                <span>
                                    DC
                                </span>
                                <ul>
                                    <li v-for="elem in dc">
                                        <a href="">
                                            {{ elem }}
                                        </a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                        <div class="my-col">
                            <div>
                                <span>
                                    SITES
                                </span>
                                <ul>
                                    <li v-for="elem in sites">
                                        <a href="">
                                            {{ elem }}
                                        </a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="my-col-7">
                    
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer{
    min-height: 400px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    color: white;
    a{
        color: rgb(149,149,149);
        text-decoration: none;
        &:hover{
            cursor: pointer;
            color: white;
        }
    }
    .my-row{
            display: flex;
            justify-content: space-between;
            .my-col-5{
                width: calc(100%/12)*5;
                padding: 40px 0;
            }
            .my-col-7{
                width: calc(100%/12)*7;
                background-image: url('../assets/img/dc-logo-bg.png');
                background-repeat: no-repeat;
                background-position-x: 55%;
                background-position-y: 55%;
            }
            .my-col{
                flex-grow: 1;
                div{
                    padding: 10px 0;
                    ul{
                        padding: 10px 0;
                        li{
                            padding: 2px 0;
                            a{
                                padding: 2px 0;
                            }
                        }

                    }
                }
            }
        }
}
</style>
