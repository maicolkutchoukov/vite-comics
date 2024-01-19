<script>
export default {
    data() {
        return {
            comics:
            [
                'Characters',
                'Comics',
                'Movies',
                'Tv',
                'Games',
                'Videos',
                'News'
            ],
            dc:
            [
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
            shop:
            [
                'Shop DC',
                'Shop DC Collectibles'
            ],
            sites:
            [
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
        <div class="container">
            <div class="row">
                <div class="col-5 col-md-6">
                    <div class="row">
                        <div class="col-auto">
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
                        <div class="col-auto">
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
                        <div class="col-auto">
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
                <div class="col-7 col-md-6">
                    
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer{
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
    .row {
            .col-5 {
                padding: 40px 0;
            }
            .col-7 {
                background-image: url('../assets/img/dc-logo-bg.png');
                background-repeat: no-repeat;
                background-position-x: 55%;
                background-position-y: 55%;
            }
            .col-auto {
                div{
                    span {
                        font-size: 25px;
                    }
                    padding: 10px 0;
                    ul {
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
