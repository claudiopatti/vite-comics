<script>
export default {
    data () {
        return {
            mainIcone: [
            {
                image: '/img/buy-comics-digital-comics.png',
                url: '#',
                text: 'DIGITAL COMICS',
            },
            {
                image: '/img/buy-comics-merchandise.png',
                url: '#',
                text: 'DC MERCHANDISE',
            },
            {
                image: '/img/buy-comics-subscriptions.png',
                url: '#',
                text: 'SUBSCRIPTION',
            },
            {
                image: '/img/buy-comics-shop-locator.png',
                url: '#',
                text: 'COMIC SHOP LOCATOR',
            },
            {
                image: '/img/buy-dc-power-visa.svg',
                url: '#',
                text: 'DC POWER VISA',
            }
        ],

        }
    }
}
</script>

<template>
    <section class="secondSectionMain">
            <div class="container">
                <div class="infoMain">
                    <ul>
                        <li v-for="(product, index) in mainIcone " :key="index">
                            <img :src="product.image" alt="">
                            <a :href="product.url">
                                {{ product.text }}
                            </a>
                        </li>
    
                        <!-- <li>
                            <img src="/img/buy-comics-merchandise.png" alt="">

                            <a href="#">
                                DC MERCHANDISE
                            </a>
                        </li>
    
                        <li>
                            <img src="/img/buy-comics-subscriptions.png" alt="">
                            
                            <a href="#">
                                SUBDCRIPTION
                            </a>
                        </li>
                        
                        <li>
                            <img src="/img/buy-comics-shop-locator.png" alt="">

                            <a href="#">
                                COMIC SHOP LOCATOR
                            </a>
                        </li>
    
                        <li>
                            <img src="/img/buy-dc-power-visa.svg" alt="">

                            <a href="#">
                                DC POWER VISA
                            </a>
                        </li> -->
                    </ul>

                </div>

            </div>

        </section>
</template>

<style lang="scss" scoped>
/* general */


.container {
    max-width: 1000px;
    margin: 0 auto;
    display: flex;
}

.secondSectionMain {
    background-color: #0282f9;

    .container {
        justify-content: space-around;

        .infoMain {

            ul  {
                display: flex;
                list-style: none;
                height: 100%;
                align-items: center;
                padding: 30px 0;
                
                li  {
                    display: flex;
                    align-items: center;
                    padding-left: 40px;

                    a {
                        text-decoration: none;
                        color: white;
                        padding-left: 15px;
                        display: inline-block;
                        align-items: center;
                        font-size: 10px;

                    }

                    img {
                        width: 45px;
                    }

                    &:nth-child(4) img {
                                    width: 30px;
                                }
                }
            }
        }
    }
}
</style>