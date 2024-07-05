<script>
    export default{
        name: 'AppFooter',
        data(){
        return{
            comicsItems: [
                {
                    text: "Characters",
                    url: "#"
                },
                {
                    text: "Comics",
                    url: "#"
                },
                {
                    text: "Movies",
                    url: "#"
                },
                {
                    text: "TV",
                    url: "#"
                },
                {
                    text: "Games",
                    url: "#"
                },
                {
                    text: "Videos",
                    url: "#"
                }
            ],
            shopItems: [
                {
                    text: "Shop DC",
                    url: "#"
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#"
                }
            ],
            dcItems: [
                {
                    text: "Term of use",
                    url: "#"
                },
                {
                    text: "Privacy Policy (New)",
                    url: "#"
                },
                {
                    text: "Ad Choising",
                    url: "#"
                },
                {
                    text: "Advertising",
                    url: "#"
                },
                {
                    text: "Jobs",
                    url: "#"
                },
                {
                    text: "Talents Workshops",
                    url: "#"
                },
                {
                    text: "CPSC Certificates",
                    url: "#"
                },
                {
                    text: "Ratings",
                    url: "#"
                },
                {
                    text: "Shop",
                    url: "#"
                },
                {
                    text: "Contact Us",
                    url: "#"
                },
            ],
            siteItems: [
                {
                    text: "DC",
                    url: "#"
                },
                {
                    text: "Mad Magazine",
                    url: "#"
                },
                {
                    text: "DC Kids",
                    url: "#"
                },
                {
                    text: "DC Universe",
                    url: "#"
                },
                {
                    text: "DC Power Visa",
                    url: "#"
                },
            ],
            socialItems: [
                {
                    image: "footer-facebook.png",
                    url: "#",
                    text: "facebook"
                },
                {
                    image: "footer-periscope.png",
                    url: "#",
                    text: "periscope"
                },
                {
                    image: "footer-pinterest.png",
                    url: "#",
                    text: "pinterest"
                },
                {
                    image: "footer-twitter.png",
                    url: "#",
                    text: "twitter"
                },
                {
                    image: "footer-youtube.png",
                    url: "#",
                    text: "youtube"
                },
            ],


        }
}
    }
</script>

<template>
    
    <section>

        <div class="background">

            <div class="container">

                <div id="flex-wrap">
                    
                    <div class="col">

                        <nav class="navigation">
        
                            <h3>DC Comics</h3>
                            <ul>
                                <li v-for="(list, index) in comicsItems" :key="index">
                                    <a :href="list.url">{{ list.text }}</a>
                                </li>
                            </ul>
                            
                        </nav>
                        <nav class="navigation">
                            <h3>SHOP</h3>
                            <ul>
                                <li v-for="(shop, index) in shopItems" :key="index">
                                    <a :href="shop.url">{{ shop.text }}</a>
                                </li>
                            </ul>
                        </nav>
                    </div>

                    <div class="col">
                        <nav class="navigation">
                            <h3>DC</h3>
                            <ul>
                                <li v-for="(dc, index) in dcItems" :key="index">
                                    <a :href="dc.url">{{ dc.text }}</a>
                                </li>
                            </ul>
                            
                        </nav>
                    </div>

                    <div class="col">
                        <nav class="navigation">
                            <h3>SITES</h3>
                            <ul>
                                <li v-for="(site, index) in siteItems" :key="index">
                                    <a :href="site.url">{{ site.text }}</a>
                                </li>
                            </ul>
                        </nav>
                    </div>

                </div>
    
            </div>


        </div>

    </section>

    <section id="bottom-bar">
        <div class="container" id="flex-container">
            
            <a href="#" id="btn-sign">
                <span>SIGN-UP NOW!</span>
            </a>


            <div id="list-icon">
                <h3 id="title">FOLLOW US</h3>
                <nav>
                    <ul>
                        <li v-for="(social, index) in socialItems" :key="index">
                            <a :href="social.url">
                                <img :src="social.image" :alt="social.text">
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>

        </div>
    </section>
    
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.background{
    background-image: url('../assets/dc-logo-bg.png'), url('../assets/footer-bg.jpg');
    background-size: 30%, cover;
    background-position-x: 75%;
    background-position-y: center;
    background-repeat: no-repeat;
    // height: 400px;

    #flex-wrap{

        display:flex;
        gap: 25px;
        padding: 30px 0;

        .navigation{

            h3{
                color: white;
            }

            ul{
                list-style-type: none;
                padding: 10px 0;
            }

            li a{
                color:rgb(165, 165, 165);
                text-decoration: none;
                font-size: 10px;
            }
        }
    }

}

#bottom-bar{
    background-color: $bottomFooter;
    // height: 100px;
    padding: 20px 0;
    
    a{
        text-decoration: none;
        color: white;
    }

    #btn-sign{
        border: 2px solid $merch;
        padding: 12px 16px;
    }
    
    #flex-container{
        padding: 10px 0;
        @include flexbox();

        ul{
            text-decoration: none;
            list-style-type: none;
            display: flex;
            gap: 10px;
        }

        #list-icon{
            display: flex;
            align-items: center;
            gap: 10px;

            #title{
                color: $merch;
                font-weight: 600;
                padding: 0 20px;
            }

            li img{
                max-width: 80%;
            }
        }
    }
}
</style>