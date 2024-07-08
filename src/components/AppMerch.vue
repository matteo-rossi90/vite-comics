<script>
    export default{
        name: 'AppMerch',
        data(){
            return{

                merchItems: [
                    {
                        text: "DIGITAL COMICS",
                        image: "buy-comics-digital-comics.png",
                    },
                    {
                        text: "DC MERCHANDISE",
                        image: "buy-comics-merchandise.png"
                    },
                    {
                        text: "SUBSCRIPTIONS",
                        image: "buy-comics-subscriptions.png"
                    },
                    {
                        text: "COMIC SHOP LOCATOR",
                        image: "buy-comics-shop-locator.png"
                    },
                    {
                        text: "DC POWER VISA",
                        image: "buy-dc-power-visa.svg"
                    },
                ]
            }
        }
    }
</script>

<template>

    <section id="merch">
        <div class="container">

            <!-- icone con menu per i prodotti -->
            <nav>
                <ul>
                    <li v-for="(merch, index) in merchItems" :key="index">
                        <img :src="merch.image" :alt="merch.text">
                        <a href="#">{{ merch.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </section>


</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

#merch{
    background-color: $merch;
    // height: 150px;
    padding: 30px;

        ul{
            list-style-type: none;
            @include flexbox();
            gap: 30px;
            padding: 10px;
            
            li {
                @include flexbox();
                gap: 10px;

                img{
                    height: 40px;
                    width: 40px; 
                    object-fit: contain;
                }
                a{
                    text-decoration: none;
                    color: white;
                    font-size: 13px;
                }
            }
        }
    
}

</style>