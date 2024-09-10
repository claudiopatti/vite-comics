<script>
export default {
    data() {
      return {
        dcComicsFooter: [
            {   
                title: 'Characters',
                url: '#',
                active: false,
            },
            {
                title: 'Comics',
                url: '#',
                active: false,
            },
            {
                title: 'Movies',
                url: '#',
                active: false,
            },
            {
                title: 'Tv',
                url: '#',
                active: false,
            },
            {
                title: 'Games',
                url: '#',
                active: false,
            },
            {
                title: 'Collectibles',
                url: '#',
                active: false,
            },
            {
                title: 'Videos',
                url: '#',
                active: false,
            },
        ],

        dcFooter: [
            {   
                title: 'Terms Of Use',
                url: '#',
                active: false,
            },
            {
                title: 'Privacy policy (New)',
                url: '#',
                active: false,
            },
            {
                title: 'Ad Choices',
                url: '#',
                active: false,
            },
            {
                title: 'Adverting',
                url: '#',
                active: false,
            },
            {
                title: 'Jobs',
                url: '#',
                active: false,
            },
            {
                title: 'Subscriptions',
                url: '#',
                active: false,
            },
            {
                title: 'Talent Workshops',
                url: '#',
                active: false,
            },
            {
                title: 'CPSC Certicates',
                url: '#',
                active: false,
            },
            {
                title: 'Ratings',
                url: '#',
                active: false,
            },
            {
                title: 'Shop Help',
                url: '#',
                active: false,
            },
            {
                title: 'Contact Us',
                url: '#',
                active: false,
            },
        ],
        sitesFooter: [
            {
                title: 'DC',
                url: '#',
                active: false,
            },
            {
                title: 'MAD Magazine',
                url: '#',
                active: false,
            },
            {
                title: 'DC Kids',
                url: '#',
                active: false,
            },
            {
                title: 'DC Universe',
                url: '#',
                active: false,
            },
            {
                title: 'DC Power Visa',
                url: '#',
            }
        ]
      };
    }
}
</script>

<template>
     <footer>
        <section class="fistSectionFooter">
            <div class="container">
                <div class="containerListInfofooter">
                    <div class="listInfoFooter">
                        <h3>
                            DC COMICS
                        </h3>
                        <ul>
                            <li v-for="(comic, index) in dcComicsFooter" :key="index">
                                <a :href="comic.url">
                                    {{ comic.title }}
                                </a>
                            </li>
                            <!-- <li>
                                <a href="#" >
                                    COMICS
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    MOVIES
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    TV
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    GAMES
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    COLLECTIBLES
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    VIDEOS
                                </a>
                            </li> -->
                        </ul>
        
        
                        <h3>
                            SHOP
                        </h3>
                        <ul>
                            <li>
                                <a href="#">
                                    Shop DC
                                </a>
                            </li>
                            <li>
                                <a href="#" >
                                    Shop Dc Collectibles
                                </a>
                            </li>
                        </ul>
                    </div>
        
                    <div class="listInfoFooter">
                        <h3>
                            DC
                        </h3>
                        <ul>
                            <li v-for="(contact, index) in dcFooter" :key="index">
                                <a :href="contact.url">
                                    {{ contact.title }}
                                </a>
                            </li>
                            <!-- <li>
                                <a href="#">
                                    Terms Of Use
                                </a>
                            </li>
                            <li>
                                <a href="#" >
                                    Privacy policy (New)
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Ad Choices
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Adverting
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Jobs
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Subscriptions
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Talent Workshops
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    CPSC Certicates
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Ratings
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Shop Help
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Contact Us
                                </a>
                            </li> -->
                        </ul>
                    </div>
                    
                    <div class="listInfoFooter">
                        <h3>
                            SITES
                        </h3>
                        <ul>
                            <li v-for="(dc, index) in sitesFooter" :key="index">
                                <a :href="dc.url">
                                    {{ dc.title }}
                                </a>
                            </li>
                            <!-- <li>
                                <a href="#">
                                    DC
                                </a>
                            </li>
                            <li>
                                <a href="#" >
                                    MAD Magazine
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    DC Kids
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    DC Universe
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    DC Power Visa
                                </a>
                            </li> -->
                        </ul>
                    </div>
                </div>
    

                <img src="/img/dc-logo-bg.png" alt="">

            </div>
        </section>

        <section class="secondSectionFooter">
            <div class="container">
                <div class="buttonFooter">
                    <button>
                        SING-UP NOW!
                    </button>
                </div>

                <div class="iconeFooter">
                    <h3>
                        FOLLOW US
                    </h3>

                    <a href="#">
                        <img src="/img/footer-facebook.png" alt="">
                    </a>

                    <a href="#">
                        <img src="/img/footer-twitter.png" alt="">
                    </a>

                    <a href="#">
                        <img src="/img/footer-youtube.png" alt="">
                    </a>

                    <a href="#">
                        <img src="/img/footer-pinterest.png" alt="">
                    </a>

                    <a href="#">
                        <img src="/img/footer-periscope.png" alt="">
                    </a>

                </div>

            </div>

        </section>
    </footer>
</template>

<style lang="scss" scoped>
/* general */


.container {
    max-width: 1000px;
    margin: 0 auto;
    display: flex;
}


/* footer  */

.fistSectionFooter {
    background-image: url("/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;

    .container{
        padding: 30px 0;
        display: flex;
        justify-content: space-between;

        img{
            width: 400px;
        }

        .containerListInfofooter {
            display: flex;

            .listInfoFooter {
                list-style: none;

                h3 {
                    color: white;
                }

                ul {
                    list-style: none;
                    padding: 15px 30px 15px 0;

                    li  {
                        padding: 5px 0;

                        a {
                            text-decoration: none;
                            color: #8c8d8d;
                            font-size: 15px
                        }
                    }
                }
            }

        }
    }

}

.secondSectionFooter {
    background-color: #303030;

    .container{
        padding: 20px 0;
        justify-content: space-between;
        align-items: center;

        .buttonFooter button{
            background-color: #303030;
            color: white;
            padding: 10px;
            border: 2px solid #0282f9;
            font-weight: bold;
        }

        .iconeFooter {
            display: flex;
            align-items: center;

            h3 {
                color: #0282f9;
                font-size: 15px;
            }

            a {
                padding-left: 15px;

                img {
                    width: 25px;
                }
            }
        }
    }
}
</style>