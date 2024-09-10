<script>
export default {
    data() {
      return {
        titlesHeader: [
            {
                title: 'CHARACTERS',
                url: '#',
                active: false,
            },
            {
                title: 'COMICS',
                url: '#',
                active: true,
            },
            {
                title: 'MOVIES',
                url: '#',
                active: false,
            },
            {
                title: 'TV',
                url: '#',
                active: false,
            },
            {
                title: 'GAMES',
                url: '#',
                active: false,
            },
            {
                title: 'COLLECTIBLES',
                url: '#',
                active: false,
            },
            {
                title: 'VIDEOS',
                url: '#',
                active: false,
            },
            {
                title: 'FANS',
                url: '#',
                active: false,
            },
            {
                title: 'NEWS',
                url: '#',
                active: false,
            },
            {
                title: 'SHOP',
                url: '#',
                active: false,
            },
        ],

      };
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="imageContainer">
                <img src="/img/dc-logo.png" alt="logo dc">
            </div>
    
            <div class="infoHeader">
                <ul>
                    <li v-for="(title, index) in titlesHeader" :key="index"
                    :class="{
                        'active' : title.active
                    }">
                        <a :href="title.url">
                            {{title.title}}
                        </a>
                    </li>
                    <!-- <li id="active">
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
                    </li>
                    <li>
                        <a href="#">
                            FANS
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            NEWS
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            SHOP
                        </a>
                    </li> -->
                </ul>
            </div>

        </div>
    </header>
</template>

<style lang="scss" scoped>
/* general */


.container {
    max-width: 1000px;
    margin: 0 auto;
    display: flex;
}


/* header  */

header .container {
    justify-content: space-between;
}

.imageContainer {
    img {
        width: 60px;
        margin: 10px 0;
    }
}

.infoHeader {
    ul  {
        display: flex;
        list-style: none;
        height: 100%;
        align-items: center;
        padding-left: 0;
        font-weight: bold;
        
        li{
            a {
                text-decoration: none;
                color: black;
                margin-left: 25px;
                display: inline-block;
                font-size: 10px;

            }
        }

        .active a {
            color: #0282f9;
            height: 100%;
            border-bottom: 5px solid #0282f9;
        }
    }
}
</style>